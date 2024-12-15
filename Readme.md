technologyone

Numeric Converter Application:
This is a simple ASP.NET Core Razor Pages application that converts numeric dollar amounts into their text representations (e.g., $123.45 becomes "ONE HUNDRED TWENTY-THREE DOLLARS AND FORTY-FIVE CENTS").

Prerequisites:
Before you begin, ensure you have the following installed on your system:
.NET 9.0 or later

Download and install from Microsoft's .NET website.
   
Integrated Development Environment (IDE):
   Recommended: Visual Studio 2022 (with the ASP.NET and web development workload).

Git (optional, if cloning from a repository):
   Download and install from Git's website.

Building the Solution:
Follow these steps to build the application:
Clone the Repository (if applicable):
   git clone <repository-url>
   cd <repository-folder>

Open the Solution:
   Launch Visual Studio
   Open the .sln file located in the root folder of the project.

Restore Dependencies:
   Visual Studio will automatically restore dependencies using NuGet.
   Alternatively, you can use the terminal in the project directory:
   dotnet restore

Build the Project:
Click on Build > Build Solution in Visual Studio, or run:
   dotnet build
   
Hosting the Application:
Run the application on your local machine:
   In Visual Studio, press Ctrl + F5 or click Debug > Start Without Debugging to launch the application.
   The application will open in your default web browser at a URL similar to:
      https://localhost:5001
      or
      http://localhost:5000
   Alternatively, use the terminal to start the application:
      dotnet run
   The output will display the local URLs where the application is running.

Using the Numeric Converter:
Enter a dollar amount in the input field (e.g., 123.45).
Click the Convert button.

Viewing the Results:
The numeric input will be converted to its text representation and displayed below the form.
If the input is invalid or exceeds limits, an error message will be displayed.
