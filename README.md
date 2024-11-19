Guardian Save: Banking Transaction Prototype 🚀
📚 Project Overview
Guardian Save is a web-based application designed for secure transaction requests between a guardian and a dependent. It demonstrates a simple yet effective account management system, making it a practical solution for educational and prototype use.

🛠️ Features
Role-based Access: Separate dashboards for guardians and dependents.
Transaction Validation: Guardians approve or reject transaction requests.
Dynamic Data Handling: Interacts with a MySQL database for user and transaction management.
⚙️ Prerequisites
Environment Setup:

Install a local server environment like XAMPP or WAMP.
Ensure PHP, MySQL, and Apache are properly configured.
Database Configuration:

Import the provided SQL file (guardian_safe.sql) into MySQL.
Ensure the database is named test and contains the following tables:
parents: For guardian data (e.g., token ID, UPI PIN).
children: For dependent data (e.g., username, parent token ID).
🚀 How to Run
Step-by-Step Flow
Home Page

Open index.html in your browser.
New User?
Navigate to the Registration Page to create a username and role (Guardian or Dependent).
Login

Use your credentials to log in.
Guardian: Redirects to dashboarda.php.
Dependent: Redirects to dashboarda.php.
Dependent Actions

After logging in, the dependent can submit transaction requests via dashboardb.php.
Fill in required details (e.g., amount, reason) and send for guardian approval.
Guardian Actions

Log in to dashboarda.php to view pending requests.
Click on a request to navigate to approve.php.
In approve.php, approve or reject requests.
Approval Flow: If approved, you must validate the action using your UPI PIN.
Approval and Completion

Upon UPI PIN validation, the request status is updated in the database, and the dependent is notified.
🗂️ File Structure
Guardian-Safe ├── index.html # Entry point of the application ├── register.php # User registration logic ├── dashboarda.php # Guardian dashboard ├── dashboardb.php # Dependent dashboard ├── approve.php # Guardian request approval page ├── transaction.php # Transaction completion page ├── error.php # Error handling page ├── guardian_safe.sql # Database schema

💡 Future Enhancements
Enhanced Security: Hash UPI PINs and implement secure sessions.
Responsive Design: Optimize for mobile and tablet devices.
Notifications: Add email or SMS notifications for guardians.
Dashboard Features: Include request history and visual analytics.
🎯 Key Takeaways
Languages & Tools: HTML, CSS, JavaScript, PHP, MySQL.
Learning Outcome: Gained hands-on experience in backend logic and database integration.
Applications: Demonstrates knowledge of transaction handling and user management.
👨‍💻 Author
Yuvaraju
Enthusiastic Computer Science student passionate about solving real-world problems through programming and development.

