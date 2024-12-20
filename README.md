Role-Based Access Control (RBAC) System
This project implements a Role-Based Access Control (RBAC) system using React.js. It allows different user roles such as System Administrator, Data Analyst, and Compliance Officer to access and manage specific parts of the system based on their permissions. Users can log in and be redirected to their respective dashboards where they can manage roles, access sales data, handle permission requests, and more.
Note: Since this project does not use a backend framework, the changes made by the user does not get stored. It will be erased if the website is refreshed and will come to its initial state. Hence, DO NOT refresh the pages in the middle of use.

Table of Contents
•	Introduction
•	Features
•	Technologies
•	Project Structure
•	Routing and Navigation
•	Development
•	Running project locally
1.	Introduction
The Role-Based Access Control (RBAC) system is designed to streamline user management and permissions within an organization. The application dynamically adjusts content and access rights based on the role of the user, ensuring that each user can only access the features and data they are authorized to use.
Key Features:
1.	User Roles & Permissions:
o	Different users are assigned specific roles such as System Admin, Data Analyst, and Compliance Officer.
o	Roles determine access to the system’s features and data.
2.	Sales Data Dashboard:
o	Data Analysts can access and analyze sales data, generating reports, viewing graphs, and tracking trends.
3.	Role Management:
o	System Admins can assign and modify roles and permissions to users, ensuring appropriate access control across the platform.
4.	Permission Request Management:
o	Users can submit permission requests, which System Admins can approve or deny based on the organizational needs.
5.	Responsive UI:
o	The application is built using Material-UI (MUI) and is fully responsive, ensuring a seamless experience across desktop, tablet, and mobile devices.
6.	Mock API for Development:
o	The project includes a mock API that simulates backend functionality, making it easier to test and develop features without needing a live backend.
2.	Features
The RBAC system is designed to offer a set of functionalities tailored to each user's role, ensuring a smooth workflow for managing permissions, analyzing data, and handling system tasks.
i.	Role Management:
•	System Admins can:
o	Assign roles (e.g., Data Analyst, Compliance Officer, etc.) to users.
o	Modify user permissions and review role-related activities.
o	Ensure compliance with internal policies by managing who has access to specific system areas.
•	Compliance officer can:
o	View user roles.




ii.	Sales Data Dashboard:
•	Data Analysts have access to the Sales Data section, where they can:
o	View and analyze sales trends, generate reports, and interpret key metrics.
o	Use interactive charts and graphs to visualize sales performance over time.
iii.	Permission Requests:
•	Users in different roles can submit permission requests if they need access to additional resources or areas.
•	System Admins have the ability to review and approve or reject these requests, ensuring only authorized users gain elevated permissions.
iv.	Compliance Monitoring:
•	Compliance Officers ensure that user permissions and actions within the system comply with internal policies and industry regulations.
•	They have oversight over system activities and can audit actions to maintain security and compliance.
v.	Responsive Design:
•	The application is built with Material-UI (MUI) for responsive layouts, ensuring that the user interface adapts across various screen sizes and devices.
vi.	Mock API:
•	A mock API is used for simulating the backend during development. It returns predefined responses for various actions such as logging in, viewing data, and managing roles.
•	This setup allows developers to test and debug the front-end application without needing a live backend.
3.	Technologies
This RBAC system is built using the following technologies:
•	React.js: A JavaScript library for building user interfaces. It enables the creation of dynamic and interactive web pages with minimal code.
•	React Router: For managing navigation and routing in the application. It ensures that the correct components are displayed based on the current URL path.
•	Material-UI (MUI): A React UI framework that provides pre-built, customizable components for building modern, responsive user interfaces.
•	Bootstrap: For additional responsive design utilities and grid layout systems.
•	Mock API: The backend is simulated using a mock API, making it easy to develop and test the application without relying on a live backend service.
•	CSS: For global styles and additional customization to enhance the look and feel of the application.
4.	Project Structure
The project follows a modular structure where each feature or page is encapsulated in its own component. Below is a breakdown of the project structure:

/rbac-system
  /public
    index.html                  # The HTML template used by React
  /src
    /Components
      /LoginPage.js              # Login page component, handles user authentication
      /DataAnalyst.js            # Data Analyst Dashboard component
      /ComplianceOfficer.js      # Compliance Officer Dashboard component
      /SystemAdmin.js            # System Admin Dashboard component
      /SalesData.js              # Sales data analysis and visualization component
      /RoleManagement.js         # Manage user roles and permissions
      /PermissionRequest.js      # Submit and review permission requests
      /mockApi.js                # Simulated API used for testing and development
    /App.js                      # Main app file containing routing logic
    /index.js                    # Entry point for the app
    /index.css                   # Global CSS styles
  package.json                   # Project dependencies and scripts
  README.md                      # This README file
Key Components:
•	App.js: The main component that defines the application’s layout and routing logic. It uses React Router to manage navigation between different pages based on the user’s role.
•	mockApi.js: Contains mock API data and functions to simulate backend interactions, such as logging in, fetching data, and managing roles and permissions.
•	index.js: The entry point of the React application. It renders the app inside the root element of the index.html file and sets up mock API data for development.
•	index.css: Global CSS file that provides basic styles, including font settings and general layout tweaks.

5.	Routing & Navigation
The application uses React Router to handle routing between different pages. The routing is dynamic based on the user’s role, allowing access to specific features only for authorized users.
The available routes in the application are:
•	/: Login Page (authentication)
•	/DataAnalyst: Data Analyst Dashboard (view and analyze sales data)
•	/ComplianceOfficer: Compliance Officer Dashboard (monitor permissions and system compliance)
•	/SystemAdmin: System Admin Dashboard (manage user roles, permissions, and requests)
•	/SalesData: Sales Data Page (analyze and visualize sales data)
•	/RoleManagement: Role Management Page (assign and modify user roles)
•	/PermissionRequest: Permission Request Page (submit and review permission requests)
The System Admin has access to all pages, while the Data Analyst and Compliance Officer can only access certain parts of the system, depending on their roles.

6.	Development
Environment Setup
1.	Node.js: Ensure Node.js is installed on your machine. You can download it here.
2.	Package Manager: Use either npm to install dependencies.

7.	Running the Project Locally
To run the application locally, follow these steps:
1.	Download and extract the zip file.

2.	Move your terminal space to rbac folder.

cd rbac

3.	Install the dependencies using 
npm install
4.	Start the development server using

npm start

5.	Access the application in your browser at address

http://localhost:3000



