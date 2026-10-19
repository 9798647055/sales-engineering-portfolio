# Punjab National Bank (PNB): Automated Loan Collection Calls

| | |
|---|---|
| **Client** | Punjab National Bank (PNB) |
| **Employer** | Sarv Group |
| **Industry** | Banking / BFSI (loan collections) |
| **Solution** | Automated outbound loan-due reminder calls, with call reports in both the Sarv and PNB portals |
| **Channel** | Voice: automated outbound calls, plus manual agent follow-up |
| **Status** | Implemented |
| **My role** | Sales: client discussions, requirement gathering and solution proposal |
| **Year** | _To be added_ |

## One-line pitch
When a loan payment falls due, the bank's portal triggers an **automated call** to the account holder reminding them of the amount and due date. Customers who do not pick up are reported straight to the bank's agents, who follow up manually.

## The problem
PNB needed to remind a large number of loan account holders about outstanding amounts and due dates, without agents calling every customer. They also needed to know **who had picked up and who had not**, so that agents could spend their time only on the customers who still needed a personal call.

## The solution
- **Automated reminder call:** triggered from the PNB portal, the Sarv platform calls the loan account holder and reminds them to pay a specific due amount by a specific date.
- **Call report:** if the customer does not pick up, a report is generated automatically in the **Sarv portal**.
- **Report pushed to PNB:** the same report is sent to the **PNB online portal**, where a live PNB agent can see whether the customer picked up.
- **Manual follow-up:** for customers who did not pick up, the PNB agent calls the loan account holder personally to request payment.

```
PNB portal -> Due date reached -> Sarv platform -> Automated call to loan holder
   -> Picked up: reminder played
   -> Not picked up: report in Sarv portal -> report pushed to PNB portal -> PNB agent calls manually
```

## Business value (expected, to be confirmed with results)
- Routine due-date reminders are automated, so agents are not tied up with them
- Agents focus on customers who did not respond to the automated call
- The bank has a clear, shared view of who picked up and who did not
- Faster and more consistent follow-up on outstanding loan payments

## Documents in this folder
| File | What it covers |
|---|---|
| [requirements.md](requirements.md) | Client's problem, needs and scenarios |
| [proposed-solution.md](proposed-solution.md) | What was proposed and why |
| [architecture/solution-architecture.md](architecture/solution-architecture.md) | Architecture and flow diagrams |
| [integration/call-and-report-flow.md](integration/call-and-report-flow.md) | Call trigger, reporting and agent follow-up logic |
| [implementation-plan.md](implementation-plan.md) | Approach and responsibilities |
| [sales-playbook.md](sales-playbook.md) | Pitch, discovery questions, objection handling |
| [outcome.md](outcome.md) | Business value, results and lessons learned |

> Items marked _To be added_ are not yet captured and should be filled in from the deal records.
