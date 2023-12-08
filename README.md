ToDoApp
ToDoApp is a simple task management application built with Angular 15, .NET Core, and Microsoft SQL Server. It allows users to create, update, and delete tasks, providing a basic interface to manage their to-do list.

Table of Contents
Prerequisites
Getting Started
Running the Application
Testing
Usage
Assumptions and Decisions
Prerequisites
Before running the application, ensure that you have the following prerequisites installed on your machine:

Node.js and npm
Angular CLI (npm install -g @angular/cli)
Visual Studio 2022
Microsoft SQL Server
Getting Started
Clone the repository:
https://github.com/BadriManjuBhargavi/Assign.git


Navigate to the project directory:

cd ToDoApp
Install Angular dependencies:

cd ToDoApp.Web
npm install
Install .NET dependencies:

cd ToDoApp.API
dotnet restore
Create a SQL Server database named 'ToDoAppDb'.

Update the connection string in appsettings.json in the ToDoApp.API project with your SQL Server details.

Running the Application
Run the API (from the ToDoApp.API directory):

dotnet run
The API will be available at 'http://localhost:5031'.

Run the Angular app (from the ToDoApp.Web directory):

ng serve
The Angular app will be available at 'http://localhost:4200'.

Testing
Open Visual Studio and navigate to Test > Test Explorer.
Click the "Run All Tests" button to execute backend tests.
Usage
Open your browser and navigate to http://localhost:4200.
Use the interface to manage your to-do list:
Click "Add Task" to create a new task.
Click "Edit" to update a task.
Click "Delete" to remove a task.
Assumptions and Decisions
Database Connection: The application assumes a SQL Server database named 'ToDoAppDb'. The connection string is set in 'appsettings.json' for the API.

Frontend Styling: Bootstrap is used for basic styling. You can customize the styles based on your preferences.

Testing Frameworks: NUnit is used for backend testing. Feel free to choose other testing frameworks if preferred.

Cross-Origin Resource Sharing (CORS): CORS is configured to allow requests from 'http://localhost:4200'. Update it based on your deployment scenario.

Feel free to reach out if you have any questions or encounter issues during setup or usage. Enjoy managing your tasks with ToDoApp!

