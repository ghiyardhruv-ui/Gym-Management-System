IRONPULSE FITNESS — GYM MANAGEMENT WEBSITE
==========================================

PROJECT TYPE
Frontend-only Gym Management Website using HTML5, CSS3, JavaScript and
browser LocalStorage. No PHP, Java, Node.js, server-side code or SQL database
is required.

ORIGINAL PAGES RETAINED AND UPGRADED
USER SIDE:
1. user-home.html       — Public home page with live local totals.
2. user-about.html      — Gym story and values.
3. user-plans.html      — Membership plans loaded from LocalStorage.
4. user-trainers.html   — Active trainer profiles loaded from LocalStorage.
5. user-contact.html    — Contact enquiry form saved in LocalStorage.

ADMIN SIDE:
6. admin-login.html     — Demo-only admin login.
7. admin-dashboard.html — Dynamic overview cards and management links.
8. admin-members.html   — Add, edit, search and delete member records.
9. admin-plans.html     — Add, edit and delete membership plans.
10. admin-messages.html — Review enquiries, update status and delete.

NEW PAGES ADDED
11. index.html            — Entry page that opens the public home page.
12. user-register.html    — Public member registration form.
13. admin-trainers.html   — Trainer CRUD (add, view, edit, delete).
14. admin-attendance.html — Mark and review daily attendance.
15. admin-payments.html   — Add and review paid/pending payment records.
16. admin-reports.html    — Dynamic summary cards and simple bar reports.

NEW JAVASCRIPT FILES
- js/storage.js
  Creates starter records the first time the website opens, reads and writes
  the project data, and generates record IDs. The LocalStorage key is
  "ironpulse_gym_data_v1".

- js/app.js
  Contains the page interactions, form validation, rendering, CRUD actions,
  demo admin login, attendance, payment calculations and reports.

STYLES
- style.css retains the original dark background, lime accent, typography,
  cards and responsive layout. Additional styles support admin tables,
  form notices, status labels, reports and mobile navigation.

HOW TO RUN
1. Extract the ZIP folder.
2. Open the extracted folder in Visual Studio Code.
3. Recommended: install/use the VS Code Live Server extension.
4. Right-click index.html and choose "Open with Live Server".
5. The public website opens. Use the top navigation to browse user pages.
6. Select Admin in the public navigation to open the admin login page.
7. Use the demo credentials below.

DEMO ADMIN LOGIN
Username: admin
Password: IronPulse@123

IMPORTANT: This login is only a demonstration. The username and password are
written in client-side JavaScript and can be viewed by anyone. It is NOT secure
authentication and must not be used to protect real or private information.

FEATURES
- Members: create, update, search and delete member records.
- Plans: create, update, activate/deactivate and delete plans. A plan assigned
to a member cannot be deleted until members are moved to another plan.
- Trainers: create, update, activate/deactivate and delete trainer profiles.
- Attendance: record Present or Absent for a member and date; duplicate
member/date entries are prevented.
- Payments: record amount, date, method and Paid/Pending status. Marking a
payment Paid also changes that member's status to Active.
- Reports: calculate totals from current browser records; charts show members
by plan and paid revenue for the last six months.
- Registration: visitors can submit a member registration request. New
registrations are saved with Pending status for admin review.
- Enquiries: contact form submissions are saved and can be triaged by admin.

LOCALSTORAGE NOTES AND LIMITATIONS
- Data is stored only in the browser profile and site origin where the project
is opened. It is not stored in a central database and is not synchronized to
other devices or browsers.
- Use the same Live Server address each time. Opening HTML files directly with
file:// may behave differently across browsers.
- Clearing browser site data can erase all project records.
- Do not enter real passwords, sensitive personal information or card/bank
information into this demo.
- Payment records are manual examples. No payment gateway or money transfer
is connected.
- Contact enquiries are saved locally. No email is sent.
- The admin demo login is not secure. A browser-only website cannot provide
production-grade authentication or protect data from its users.
- Reports are only as accurate as the records entered into this browser.

RESETTING THE SAMPLE DATA
After logging in as admin, use "Reset Sample Data" on the dashboard. This
replaces all changes in this browser with the starter sample records.

TECHNOLOGY
HTML5 • CSS3 • Vanilla JavaScript • Browser LocalStorage • VS Code Live Server
