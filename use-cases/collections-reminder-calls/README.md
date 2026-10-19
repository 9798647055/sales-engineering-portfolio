# Use Case: Collections Reminder Calls with Agent Follow-up

## Pattern
A lender's system triggers an automated reminder call when a payment is due. If the customer picks up, they hear the amount and due date. If not, the outcome is reported to the lender's agents, who follow up manually.

```
Lender portal -> Payment due -> Automated call -> Picked up: reminder played
                                              -> Not picked up: report -> Agent calls manually
```

## Where it fits
| Industry | Trigger | Recipient |
|---|---|---|
| Banking | Loan EMI due | Loan account holder |
| NBFC / fintech | Repayment due | Borrower |
| Insurance | Premium due | Policyholder |
| Credit cards | Payment due | Cardholder |
| Utilities | Bill due | Customer |

## Typical building blocks
- Call trigger from the lender's portal
- Automated outbound call with a due amount and date message
- Outcome report (picked up or not), visible to the lender's agents
- Manual follow-up by agents for customers who were not reached

## Projects using this pattern
| Project | Industry |
|---|---|
| [PNB: Automated Loan Collection Calls](../../pnb-loan-collection-calls/README.md) | Banking / BFSI |
