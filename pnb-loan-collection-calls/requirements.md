# Requirements: Punjab National Bank (PNB)

## Business context
PNB is a large public sector bank in India. A key part of loan management is reminding account holders about due amounts and dates, and following up when payments are outstanding.

## Client pain points
- Reminding every loan account holder by manual calls is slow and does not scale
- Agents cannot easily tell which customers received the reminder and which did not
- Follow-up effort should go to customers who did not respond to the reminder

## Client needs
| # | Need | Priority |
|---|---|---|
| 1 | **Automatically call** customers who have taken a loan from PNB when a payment is due | High |
| 2 | Calls placed from a **dedicated number series** (1400 series, as stated in the requirement, _to be confirmed_) | High |
| 3 | The call **reminds the customer** of the due amount and the date to pay | High |
| 4 | Calls are **initiated from the PNB portal** | High |
| 5 | If the customer does not pick up, a **report is generated automatically** in the Sarv portal | High |
| 6 | The same report is **pushed to the PNB online portal** | High |
| 7 | **PNB live agents** can see whether the customer picked up | High |
| 8 | Agents **manually call** customers who did not pick up | High |

## Scenarios
| # | Scenario | Expected behaviour |
|---|---|---|
| 1 | A loan payment is due | The PNB portal triggers an automated call through the Sarv platform |
| 2 | Customer picks up | The reminder is played: due amount and date |
| 3 | Customer does not pick up | A report is created in the Sarv portal and pushed to the PNB portal |
| 4 | Agent reviews the report | The agent sees the customer did not pick up and calls manually to request payment |

## Success criteria
- Due-date reminder calls go out automatically
- Not-picked-up customers are visible to PNB agents without manual tracking
- Agents spend their time on follow-up, not on routine reminders

## Information still to capture
- Volume of calls per day or month
- Calling hours and the rules for collection calls
- Languages for the reminder message
- Number of retries, if any
