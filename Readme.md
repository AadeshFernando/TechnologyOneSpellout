Numeric Converter Application

This is a simple ASP.NET Core Razor Pages application that converts numeric dollar amounts into their text representations (e.g., $123.45 becomes "ONE HUNDRED TWENTY-THREE DOLLARS AND FORTY-FIVE CENTS").

Prerequisites

Before you begin, ensure you have the following installed on your system:

.NET 6.0 SDK or later

Download and install from Microsoft's .NET website.

Integrated Development Environment (IDE)

Recommended: Visual Studio 2022 (with the ASP.NET and web development workload).

Git (optional, if cloning from a repository)

Download and install from Git's website.

Building the Solution

Follow these steps to build the application:

Clone the Repository (if applicable):

git clone <repository-url>
cd <repository-folder>

Open the Solution:

Launch Visual Studio.

Open the .sln file located in the root folder of the project.

Restore Dependencies:

Visual Studio will automatically restore dependencies using NuGet.

Alternatively, you can use the terminal in the project directory:

dotnet restore

Build the Project:

Click on Build > Build Solution in Visual Studio, or run:

dotnet build

Hosting the Application

There are two primary ways to host this application: locally or on a web server.

1. Hosting Locally

Run the application on your local machine:

In Visual Studio, press Ctrl + F5 or click Debug > Start Without Debugging to launch the application.

The application will open in your default web browser at a URL similar to:

https://localhost:5001

or

http://localhost:5000

Alternatively, use the terminal to start the application:

   dotnet run

The output will display the local URLs where the application is running.

2. Hosting on a Web Server

To deploy the application to a production server, follow these steps:

Publish the Application:

In Visual Studio, right-click the project in Solution Explorer, then select Publish.

Follow the publishing wizard to publish the application to a folder.

Alternatively, use the terminal:

dotnet publish -c Release -o ./publish

The compiled files will be in the ./publish directory.

Host on IIS (Windows):

Install IIS and the ASP.NET Core Hosting Bundle.

Configure a new site in IIS, pointing to the ./publish folder.

Host on Linux/NGINX:

Install the .NET Runtime and configure NGINX as a reverse proxy.

Point the server to the published directory.

For detailed hosting instructions, refer to the official Microsoft documentation.

Interacting with the Application

Once the application is running, follow these steps:

Open the Application:

Visit the application in your browser using the hosted URL (e.g., https://localhost:5001).

Use the Numeric Converter:

Enter a dollar amount in the input field (e.g., 123.45).

Click the Convert button.

View the Results:

The numeric input will be converted to its text representation and displayed below the form.

If the input is invalid or exceeds limits, an error message will be displayed.