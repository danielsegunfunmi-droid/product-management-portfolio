# Internal Loan Management — Staff Loan and Repayment Tracking

**Role:** Product Manager  
**Date:** 2026 (as shown in portfolio source)  
**Users:** Staff and Finance leadership  
**Focus:** HR and finance operations  
**Status:** Shipped (as shown in portfolio source)

## 1. Product overview

Internal Loan Management is an internal HR and finance product for managing staff loan applications, approvals, active loans and monthly repayments.

The product brings the loan lifecycle into one place, replacing scattered spreadsheets and manual approval chains described in the source portfolio.

## 2. The problem

The process involved multiple connected steps: checking staff eligibility, submitting applications, obtaining finance approval, tracking active loans, calculating repayment schedules and reconciling monthly deductions.

When these steps are managed through disconnected spreadsheets and manual handoffs, it can be difficult for staff to understand their eligibility and application status, and for Finance to maintain a reliable view of outstanding balances and repayments due.

**Product problem statement:** How might we create a traceable, self-service loan-management workflow that gives staff clarity on their applications while giving Finance control and visibility over approvals, balances and repayments?

## 3. Discovery and problem framing

The source portfolio confirms that I defined eligibility logic, application flow, approval routing and repayment schedule rules. It identifies staff and the Finance lead as the main user groups.

It does not document formal interviews, process-mapping sessions, policy documents, approval matrices or the exact existing error rates. The following is a reconstruction of the discovery logic based on the workflows and user groups described in the source.

The discovery work can be explained through these areas:

- **Map the current process:** understand how staff requests were submitted, reviewed, approved, recorded and repaid.
- **Identify user needs:** determine what staff need to know before applying and what Finance needs to review and reconcile.
- **Clarify business rules:** document eligibility criteria, salary and tenure inputs, approval routing and repayment schedule rules.
- **Identify control points:** establish where authorization, status changes and audit history are required.
- **Separate user journeys:** distinguish the staff self-service experience from the finance operations experience.

The key product insight was that this was not just a loan application form. It was an end-to-end operational workflow that needed to connect eligibility, approvals, loan tracking and repayment reconciliation.

## 4. Product decisions and rationale

The source portfolio describes several concrete product decisions:

- **Create a staff self-service portal.** Staff can view salary, tenure, maximum eligible loan and loan history, reducing uncertainty before and after applying.
- **Create a dedicated Finance dashboard.** Finance can review pending applications, active loans, outstanding balances and amounts due for the month.
- **Define eligibility rules.** The source describes a maximum loan amount based on a set percentage of annual salary and staff tenure. The exact percentage is not specified and should not be disclosed or inferred.
- **Support repayment reconciliation.** Finance can mark repayments as paid after payroll deduction and export records to CSV.
- **Maintain an audit log.** Decisions and activity have a traceable history.

### Trade-offs to explain in an interview

These are product tensions implied by the solution. Confirm which ones were part of the actual decision-making:

- **Self-service versus control:** staff need transparency and autonomy, while Finance needs approval authority and oversight. Separate role-based experiences help serve both needs.
- **Automation versus exception handling:** eligibility and repayment rules can reduce manual work, but the workflow still needs a way to handle exceptions, corrections or unusual cases.
- **Convenience versus data protection:** salary and loan information is sensitive. Access should be limited to the information each role needs.
- **Operational visibility versus reporting complexity:** Finance needs a useful view of pending and active loans, but dashboards should avoid unnecessary fields and manual data maintenance.
- **System record versus payroll source of truth:** the product tracks repayments after payroll deduction. The workflow must make clear how payroll records and loan records are reconciled; the source does not specify any payroll integration.

## 5. Execution

The source portfolio describes my product contribution as defining eligibility logic, application flow, approval routing and repayment schedule rules.

The resulting workflows included:

**Staff**
- View salary and tenure information.
- View maximum eligible loan amount.
- Submit loan applications.
- Review loan history.

**Finance**
- Review pending applications.
- Track active loans and outstanding balances.
- View monthly amounts due.
- Manage repayment records.

**Repayment and audit**
- Mark repayments as paid after payroll deduction.
- Export records to CSV.
- Retain an audit log of decisions and activity.

## 6. Outcomes and impact

**Delivered:** an internal product covering staff loan applications, approvals, active-loan tracking and repayment management. The source portfolio describes it as shipped.

**Intended value:** improve visibility and consistency across the loan lifecycle, reduce dependence on scattered spreadsheets and manual approval chains, and give staff and Finance clearer workflows.

**What is not yet quantified:** no processing-time reduction, reconciliation-effort reduction, error-rate change, adoption figure or staff satisfaction result was included in the source. These should not be presented as measured outcomes without supporting evidence.

### Metrics I would use to evaluate the product

- Percentage of staff loan applications submitted through the system.
- Average time from application to decision.
- Application completeness and rework rate.
- Approval turnaround time by stage.
- Percentage of repayments reconciled by the expected date.
- Outstanding balance and overdue repayment accuracy.
- Number of manual corrections or reconciliation exceptions.
- Staff and Finance user satisfaction.
- Audit-log completeness for key loan decisions and status changes.

## 7. What this project demonstrates

Internal product management · Workflow automation · HR and finance operations · Business-rule definition · Role-based experience design · Requirements definition · Process improvement · Cross-functional collaboration · Stakeholder communication

## Evidence and validation notes

The source portfolio includes three interface visuals. It does not include the original process map, policy documentation, approval matrix, detailed access-control specification, payroll integration details or quantified operational outcomes. The discovery reconstruction and trade-off prompts above should be validated against the actual project history.
