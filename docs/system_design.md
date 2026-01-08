**SYSTEM DESIGN & ARCHITECTURE
System Overview**

The Smart Campus Facility Issue Reporting System is a web-based application designed to improve the reporting and management of facility issues within a university campus. The system allows students and staff to report facility problems by uploading an image and providing a short description. The uploaded image is analyzed using image recognition techniques to classify the type of issue and determine its severity level.

All submitted reports are stored in a database and made available through an administrative dashboard, where maintenance staff can view, track, and update the status of reported issues.

**System Actors**

The system involves the following actors:

Users (Students and Staff): Submit facility issue reports by uploading images and descriptions.

System (Backend and Machine Learning Model): Processes uploaded data, analyzes images, and classifies issues.

Admin (Maintenance Staff): Views and manages reported issues through the dashboard.

**System Architecture**

The system follows a client–server architecture model. Users interact with the frontend web interface to submit issue reports. The frontend sends the uploaded image and description to the backend server for processing. The backend server communicates with the machine learning component to classify the issue type and severity.

All report data, including images, predictions, and status updates, are stored in a database. The admin dashboard retrieves data from the database to display reported issues and allow maintenance staff to manage repairs.

**System Workflow
User Workflow**

The user accesses the web application.

The user uploads an image of the facility issue.

The user enters a short description of the problem.

The user submits the issue report.

**System Workflow**

The backend server receives the image and description.

The image is processed by the machine learning model.

The system predicts the issue category and severity level.

The report data is stored in the database.

**Admin Workflow**

The admin logs into the dashboard.

The admin views all reported facility issues.

The admin updates the issue status (pending, in progress, resolved).

**Data Flow Description**

Data flows from the user interface to the backend server, where it is processed and stored. The machine learning component analyzes uploaded images and generates predictions. The admin dashboard accesses stored data to display reports and manage issue statuses.

**Technology Interaction**

Frontend: Collects user input and uploads images.

Backend: Handles application logic and communication between components.

Machine Learning Model: Classifies issue type and severity.

Database: Stores report data and system information.

Cloud Infrastructure: Hosts system components and enables scalability.

**Summary**

This system design provides a structured approach to reporting and managing campus facility issues. By combining image-based reporting, automated classification, and centralized management, the system aims to improve maintenance efficiency and transparency across the campus.
