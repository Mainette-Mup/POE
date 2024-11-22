Contract Monthly Claim System (CMCS) - README
Introduction
The Contract Monthly Claim System (CMCS) is a .NET MVC-based web application designed to streamline the submission and approval process for monthly work claims. Lecturers can submit claims for hours worked, and administrators (Programme Coordinators and Academic Managers) can review, approve, or reject these claims. The application also allows for uploading supporting documents and tracking claim statuses.
________________________________________
Getting Started
System Requirements
•	ASP.NET Core MVC Framework: Ensure your system has the necessary environment to run .NET Core MVC projects.
•	Database: SQL Server (or compatible database system).
•	Browser Compatibility: Supports modern browsers like Chrome, Edge, and Firefox.
Setting Up the Application
1.	Clone the repository using:
bash
Copy code
git clone <repository-link>
2.	Open the project in Visual Studio.
3.	Configure the database connection string in the appsettings.json file.
4.	Run the migration to set up the database schema:
bash
Copy code
dotnet ef database update
5.	Start the application:
bash
Copy code
dotnet run
6.	Access the application in your browser at http://localhost:5000.
________________________________________
Navigating the Application
1. Lecturer Dashboard
Submit New Claim:
•	Navigate to the Submit Claim page via the dashboard.
•	Enter the following details:
o	Lecturer ID
o	Hours Worked
o	Hourly Rate
•	Click the Calculate Claim button to compute the total claim amount.
•	Upload supporting documents using the Upload File button.
•	Submit the claim by clicking Submit Claim.
View Claim Status:
•	Access the Claim Status page to view a list of all previously submitted claims.
•	Each claim includes:
o	Date Submitted
o	Claim Amount
o	Status (Pending, Approved, Rejected)
o	An option to View/Edit the claim (currently non-functional).
•	Claims are displayed in a table format for easy access.
2. Admin Dashboard
Filter Claims:
•	Navigate to the Filter Claims page.
•	Specify filters:
o	Date Range: Start and End dates.
o	Lecturer: Select from a drop-down menu.
o	Claim Status: Filter by Pending, Approved, or Rejected claims.
•	Click the Filter Claims button to apply the selected criteria.
View Claims:
•	The Pending Claims section displays all claims awaiting review.
•	Each pending claim includes:
o	Lecturer Name
o	Claim Amount
o	Status
•	Actions:
o	Approve: Approve the claim.
o	Reject: Reject the claim.
________________________________________
Application Features
Lecturer Functions
1.	Submit New Claims:
o	Enter hours worked and hourly rate to calculate the total claim amount.
o	Attach supporting documents to claims.
o	Submit claims for admin review.
2.	View Claim Status:
o	Monitor the status of all submitted claims (Pending, Approved, Rejected).
________________________________________
Admin Functions
1.	Filter Claims:
o	Use filters to find claims by date, lecturer, and status.
o	Easily navigate to relevant claims.
2.	Review Claims:
o	Approve or reject claims with a single click.
o	View submitted claims, including supporting documents
Future Improvements
1.	Enhanced User Authentication:
o	Implement role-based access control (RBAC) for Lecturers and Admins.
2.	Email Notifications:
o	Send email updates to lecturers when claims are approved or rejected.
3.	Improved Document Handling:
o	Enable viewing of uploaded documents directly in the application.
4.	Claim Editing:
o	Enable lecturers to edit claims before they are reviewed by admins.
________________________________________
This revised README provides a clear overview of the CMCS as an MVC application. Let me know if additional refinements are needed!# POE
CLAIMS SYSTEM
