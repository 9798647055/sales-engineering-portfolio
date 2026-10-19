# Solution Architecture

## High-level flow
```mermaid
flowchart TD
    A["PNB portal: loan payment due"] --> B["Call request sent to Sarv platform"]
    B --> C["Automated outbound call to loan account holder"]
    C --> D{"Customer picks up?"}
    D -->|"Yes"| E["Reminder played: due amount and date"]
    D -->|"No"| F["Report generated in Sarv portal"]
    F --> G["Report pushed to PNB online portal"]
    G --> H["PNB live agent sees: not picked up"]
    H --> I["Agent calls the customer manually to request payment"]
```

## Sequence
```mermaid
sequenceDiagram
    participant PNB as PNB portal
    participant Sarv as Sarv platform
    participant Customer as Loan account holder
    participant Agent as PNB live agent
    PNB->>Sarv: Initiate call (customer, amount, due date)
    Sarv->>Customer: Automated outbound call
    alt Customer picks up
        Sarv->>Customer: Reminder: amount due and date
    else Customer does not pick up
        Sarv->>Sarv: Generate report in Sarv portal
        Sarv->>PNB: Push report to PNB portal
        Agent->>PNB: Reviews report in PNB portal
        Agent->>Customer: Manual follow-up call
    end
```

## Components
| Component | Owner | Role |
|---|---|---|
| PNB portal | PNB | Initiates call requests and shows reports to agents |
| Sarv platform | Sarv Group | Places automated calls and records the outcome |
| Sarv portal | Sarv Group | Holds the call report |
| Report push | Sarv Group + PNB | Sends the same report to the PNB portal |
| PNB live agents | PNB | Follow up manually with customers who did not pick up |

## Design notes
- **Portal-triggered:** calls start from the bank's own portal
- **Single report, two places:** the same information in the Sarv and PNB portals
- **Human follow-up where needed:** automation for the first touch, agents for the rest

## Diagram files
_Add the original draw.io / PNG architecture diagram here if one exists._
