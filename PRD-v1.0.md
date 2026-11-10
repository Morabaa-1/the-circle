# Product Requirements Document (PRD)
## The Circle — Rotating Savings Circle Management

**Document type:** Alpha Prototype PRD  
**Product:** The Circle  
**Market:** Blanchardstown, Dublin 15, Ireland  
**Version:** 1.0

### 1. Product Overview

The Circle is a lightweight digital platform designed to help members of informal rotating savings groups manage monthly contributions and payout schedules transparently.

The prototype addresses the administrative burden placed on the group organiser, who currently relies on a notebook and WhatsApp to track payments, follow up with members and coordinate monthly payouts.

### 2. Problem Statement

Managing a rotating savings circle manually creates unnecessary administrative work and limits visibility for members.

The organiser struggles to track who has paid, identify outstanding contributions and communicate whose turn it is to receive the monthly pot. Other members have no central place to check payment status or the payout schedule.

### 3. Target Users

- **Primary user — Circle organiser:** Responsible for tracking contributions, following up on outstanding payments and coordinating monthly payouts.
- **Secondary users — Circle members:** Ten friends who contribute monthly and need visibility of payment status and payout order.

Users may have limited digital literacy or use devices with small screens. The interface must therefore prioritise simplicity and readability.

### 4. Business Scenario

| Parameter | Value |
|---|---:|
| Number of members | 10 |
| Monthly contribution | €100 |
| Total monthly pot | €1,000 |
| Payout frequency | Monthly |
| Payout recipients | One member per month |
| Rotation duration | 10 months |

Every member contributes €100 monthly. One member receives the full €1,000 pot each month, following an agreed rotation until all ten members have received their turn.

### 5. Product Objectives

1. Reduce the organiser's administrative workload.
2. Provide a clear overview of monthly member contributions.
3. Improve transparency across the savings group.
4. Make the upcoming payout recipient and amount immediately visible.

### 6. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR01 | Display all ten members and their monthly payment status (Paid/Pending). | Must |
| FR02 | Display the total number of members who have paid and the amount collected. | Must |
| FR03 | Allow the organiser to mark a member's payment as received. | Must |
| FR04 | Update payment status and collection totals immediately after confirmation. | Must |
| FR05 | Display the next member scheduled to receive the monthly pot. | Must |
| FR06 | Display the next payout amount (€1,000). | Must |

### 7. Non-Functional Requirements

- **Mobile-first:** Responsive layout suitable for small smartphone screens.
- **Accessibility:** Large, readable typography, high contrast and clear status labels.
- **Simplicity:** Plain English, intuitive navigation and minimal visual clutter.
- **Performance:** Lightweight page with no unnecessary dependencies.
- **Usability:** Essential information visible immediately without navigating through menus.

### 8. Technical Scope and Constraints

The deliverable will be one self-contained `app.html` file containing HTML, CSS and JavaScript.

- No frameworks or external libraries.
- No installation requirements.
- No login or authentication.
- No backend or database.
- Ten fictional members and sample payment records stored within the file.
- No real payment processing or bank integrations.
- Payment updates are simulated within the prototype.

### 9. Out of Scope

- Real financial transactions.
- Bank account connectivity.
- Member registration and invitations.
- Automated payment reminders.
- Notifications.
- User accounts and permissions.
- Production deployment and financial regulatory authorisation.

### 10. Acceptance Criteria

The prototype will be considered successful when:

1. All ten fictional members are displayed.
2. Each member has a clearly identifiable Paid or Pending status.
3. The total number of paid members and amount collected are visible.
4. The organiser can mark a pending payment as received.
5. Payment status and collection totals update immediately.
6. The next payout recipient and €1,000 amount are clearly displayed.
7. The interface is readable and usable on a small smartphone screen.
8. All functionality works within a single HTML file without a backend.

### 11. Success Measures

The prototype should demonstrate that a member can identify who has paid, and whose turn is next, within seconds of opening the application.

The primary measure of success is reducing the organiser's reliance on manual payment tracking and repeated WhatsApp communication.

---

**Prototype Disclaimer:** The Circle is an educational alpha prototype. All members and transactions are fictional. The prototype does not process real payments or represent a live financial service.
