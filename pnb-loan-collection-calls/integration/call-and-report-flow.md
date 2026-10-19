# Call, Report and Follow-up Flow

## Flow
| Step | What happens | Next step |
|---|---|---|
| 1 | A loan payment is due, and the PNB portal initiates a call request | Step 2 |
| 2 | The Sarv platform places an automated outbound call to the loan account holder | Step 3 |
| 3 | Customer picks up | Step 4 |
| 3 | Customer does not pick up | Step 5 |
| 4 | Reminder is played with the due amount and the date to pay | End |
| 5 | A report is generated automatically in the Sarv portal | Step 6 |
| 6 | The same report is pushed to the PNB online portal | Step 7 |
| 7 | A PNB live agent sees the customer did not pick up | Step 8 |
| 8 | The agent calls the customer manually to request payment | End |

## Reminder message
| Situation | Message intent |
|---|---|
| Payment due | Reminder to pay [due amount] on [date] |

The exact wording and any customer options during the call are _to be confirmed from project records_.

## Data exchanged
| Field | Direction | Description |
|---|---|---|
| Customer phone number | PNB portal to Sarv | Number to call |
| Due amount | PNB portal to Sarv | Amount to mention in the reminder |
| Due date | PNB portal to Sarv | Date to mention in the reminder |
| Call outcome (picked up or not) | Sarv to PNB portal | Shown to live agents in the report |

No customer personal data is stored in this repository.

## Open items
- Calling-number series and its approval (1400 series stated in the requirement)
- Rules for collection calls, such as allowed calling hours and customer consent
- Whether the platform retries before reporting a customer as not picked up
- Languages for the reminder message
- Report format and how often it is pushed to the PNB portal
