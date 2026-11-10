# Product Requirements Document (PRD)
## The Circle — Rotating Savings Circle Management

**Document type:** Alpha Prototype PRD  
**Version:** 1.1  
**Market:** Blanchardstown, Dublin 15, Ireland  
**Deliverable:** Single self-contained `app.html`

### 1. Product Overview

The Circle is a lightweight digital platform designed to help members of informal rotating savings groups manage monthly contributions and payout schedules transparently.

The prototype addresses the administrative burden placed on the group organiser, who currently relies on a notebook and WhatsApp to track payments, follow up with members and coordinate monthly payouts.

The platform provides a shared overview of contributions, outstanding payments, organiser responsibilities and payout rotation.

### 2. Problem Statement

Managing a rotating savings circle manually creates unnecessary administrative work and limits visibility for members.

The organiser struggles to track who has paid, identify outstanding contributions, maintain accurate records and coordinate monthly payouts. Other members have no central place to verify payment status or see whose turn it is to receive the savings pot.

### 3. Target Users

- **Primary user — Circle organiser:** Responsible for tracking contributions, following up on outstanding payments and coordinating monthly payouts. Organising responsibility rotates among members.
- **Secondary users — Circle members:** Ten friends who contribute monthly and need visibility of payment status and payout order.

Users may have limited digital literacy or use devices with small screens. The interface must prioritise simplicity and readability.

### 4. Business Scenario

| Parameter | Value |
|---|---:|
| Number of members | 10 |
| Monthly contribution | €100 |
| Total monthly pot | €1,000 |
| Contribution frequency | Monthly |
| Payout frequency | Monthly |
| Payout recipients | One member per month |
| Rotation duration | 10 months |

All ten members contribute €100 monthly. One member receives the full €1,000 pot each month, following an agreed ten-month rotation.

Organising responsibility also rotates among members and is displayed separately from the payout schedule.

### 5. Product Objectives

1. Reduce the organiser's administrative workload.
2. Provide immediate visibility of monthly contributions and outstanding payments.
3. Improve transparency across the savings group.
4. Clearly communicate the next payout recipient and amount.
5. Maintain a visible history of completed and upcoming payouts.
6. Demonstrate the complete monthly savings-circle lifecycle.

### 6. Main Screen Requirements

The first screen must immediately display:

- Number of members who have paid and total amount collected.
- All ten members and their payment statuses.
- Members with outstanding contributions.
- Current organiser and next organiser.
- Next scheduled payout recipient and amount.
- Ten-month payout schedule.

Users must not need to navigate through menus to find this information.

### 7. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR01 | Display all ten members and their monthly payment statuses (Paid/Pending). | Must |
| FR02 | Display the number of paid members and total contributions collected. | Must |
| FR03 | Allow the organiser to mark a member's payment as received. | Must |
| FR04 | Update payment status and collection totals immediately after confirmation. | Must |
| FR05 | Display the next scheduled payout recipient and €1,000 payout amount. | Must |
| FR06 | Enable payout confirmation only when all ten contributions are recorded as received. | Must |
| FR07 | Allow the organiser to confirm the monthly payout to the scheduled recipient. | Must |
| FR08 | Display the complete ten-month payout schedule, with each month marked Received, This Month or Upcoming. | Must |
| FR09 | Allow the organiser to undo an incorrectly recorded payment, with confirmation and feedback. | Must |
| FR10 | Advance to the next month following payout confirmation and reset all payment statuses to Pending. | Must |
| FR11 | Record the completed payout recipient and month in the payout history. | Must |
| FR12 | Display the current and next month's organiser, reflecting the agreed organiser rotation. | Must |

### 8. Monthly Cycle and Business Rules

The prototype must follow this workflow:

1. All ten members are expected to contribute €100.
2. The organiser records each received payment.
3. The dashboard updates the paid-member count and total collected.
4. Once all ten payments are recorded, the payout confirmation becomes available.
5. The organiser confirms the payout to the scheduled recipient.
6. The recipient and completed month are recorded in the payout history.
7. The application advances to the next month.
8. All payment statuses reset to Pending for the new month.
9. The next payout recipient and organiser are displayed.

**Business rules:**

- Each member contributes €100 per month.
- Each monthly payout is €1,000.
- Only one member receives the pot per month.
- A payout cannot be confirmed until all ten payments are recorded.
- Payment statuses can be corrected before payout confirmation.
- Completed payout records must remain visible.
- Organiser rotation and payout rotation are separate concepts, even if the fictional group chooses to follow the same sequence.

### 9. Demo Configuration and Sample Data

The prototype must start in **Month 4 of 10**.

| Parameter | Initial state |
|---|---|
| Current month | Month 4 |
| Previous payouts | 3 completed |
| Current payout recipient | Mary |
| Current organiser | Ahmed |
| Next organiser | Sara |
| Total members | 10 |
| Members paid | 6 |
| Members pending | 4 |
| Amount collected | €600 |
| Expected collection | €1,000 |
| Next payout | €1,000 |

All ten members, names, payment records and transactions must be fictional.

The four pending payments must be available for demonstration of the payment-recording functionality.

### 10. Non-Functional Requirements

- **Mobile-first:** Responsive layout suitable for small smartphone screens.
- **Accessibility:** Large, readable typography, high contrast and clear text-based status indicators.
- **Simplicity:** Plain English, intuitive navigation and minimal visual clutter.
- **Performance:** Lightweight application with no unnecessary dependencies.
- **Usability:** Essential information visible immediately without navigating through menus.
- **Feedback:** Display short confirmation messages after user actions.

### 11. Technical Scope and Constraints

The deliverable must be one self-contained `app.html` file containing HTML, CSS and JavaScript.

- No frameworks or external libraries.
- No installation requirements.
- No login or authentication.
- No backend or database.
- Ten fictional members and sample payment records stored within the file.
- Payment updates simulated using JavaScript.
- No real payment processing or bank integrations.

### 12. Out of Scope

- Real financial transactions.
- Bank account connectivity.
- Member registration and invitations.
- Automated payment reminders.
- External notifications.
- User accounts and permissions.
- Backend persistence and real-time synchronisation.
- Production deployment and financial regulatory authorisation.

### 13. Acceptance Criteria

The prototype will be considered successful when:

1. All ten fictional members are displayed.
2. The first screen clearly shows who has paid and who is pending.
3. The number of paid members and total collected are visible.
4. The organiser can mark a pending payment as received.
5. The organiser can undo an incorrectly recorded payment.
6. Payment totals update immediately following changes.
7. The next payout recipient and €1,000 amount are clearly visible.
8. The ten-month payout schedule displays completed, current and upcoming recipients.
9. The organiser can confirm the payout once all ten members have paid.
10. The application records the completed payout and advances to the next month.
11. Payment statuses reset for the new month without deleting historical payout records.
12. Current and next organisers are visible.
13. The application is readable and usable on small smartphone screens.
14. All functionality works within one HTML file without a backend.

### 14. Success Measures

The prototype should demonstrate that:

- A member can identify who has paid and whose turn is next within seconds of opening the application.
- The organiser can track outstanding contributions without relying on a notebook or WhatsApp.
- The organiser can complete a simulated monthly payout cycle.
- Members have visibility of the full ten-month rotation.

### 15. Prototype Disclaimer

The Circle is an educational alpha prototype. All members, payment records and transactions are fictional and provided for demonstration purposes only. The prototype does not process real payments, hold customer funds or represent a live financial service.
