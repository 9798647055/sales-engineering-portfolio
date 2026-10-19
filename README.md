# Sales Engineering Portfolio

Sales Engineering portfolio showcasing CPaaS, cloud telephony, API integrations, solution architecture, customer use cases and POC implementations, from my work at **Exotel** and **Sarv Group**.

Each client has its own folder with a full write-up: requirements, proposed solution, architecture, integration logic, implementation approach, sales playbook and outcome.

> **Note:** This repository does not contain credentials, API keys, contract values or personal customer data.

## Clients
| Client | Employer | Industry | Solution | Channel | Status |
|---|---|---|---|---|---|
| [Green Line Energy](green-line-energy/README.md) | Exotel | Travel / Transportation | Telematics and driver safety automation | Voice | Implemented |
| [Dot & Key](dot-and-key/README.md) | Exotel | Beauty & Cosmetics / D2C | Order status IVR on a single number | Voice (IVR) | Implemented |
| [Swiss Beauty](swiss-beauty/README.md) | Exotel | Beauty & Cosmetics / D2C | Order status IVR with WebRTC agent calling | Voice (IVR + WebRTC) | Implemented |
| [Haptik (for Jio)](haptik-jio-voicebot/README.md) | Exotel | Telecom / Conversational AI | Recharge reminder voicebot on SIP trunk + chat-to-callback | Voice (SIP trunk, outbound API) | Implemented |
| [Punjab National Bank (PNB)](pnb-loan-collection-calls/README.md) | Sarv Group | Banking / BFSI | Automated loan collection calls with portal reporting | Voice (automated outbound) | Implemented |

## Repository structure
```
<client>/     One folder per client, each with the same set of documents
use-cases/    Reusable solution patterns across clients
templates/    Template for writing up a new client
```

## What is inside each client folder
| File | What it covers |
|---|---|
| README.md | Case-study summary |
| requirements.md | Client's problem, needs and scenarios |
| proposed-solution.md | What was proposed and why |
| architecture/ | Architecture and flow diagrams |
| integration/ | Integration logic and message mapping |
| implementation-plan.md | Approach and responsibilities |
| sales-playbook.md | Pitch, discovery questions, objection handling |
| outcome.md | Business value, results and lessons learned |

## Adding a new client
1. Copy the layout from `templates/project-template.md`
2. Create a new folder at the root for the client
3. Fill in all the documents
4. Add a row to the Clients table above, with the employer
5. Link it from the matching page under `use-cases/`
