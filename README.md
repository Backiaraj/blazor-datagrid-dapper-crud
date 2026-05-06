# Blazor DataGrid CRUD application using Dapper

This sample was created to depict DataGrid CRUD operation in SQL server database using Dapper in a Blazor server-side application.

## Prerequisites

* [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or later
* [Visual Studio Code](https://code.visualstudio.com/)

## Install

* Create a database named **BugTracker** on your SQL server, and run scripts in **SQL script** directory to create a **Bugs** table.
* Edit `appsettings.json` to set the database connection in the `BugTrackerDatabase` property.

## How to run the project

1. Clone or download this repository to a location in your system.
2. Open the solution file using the Visual Studio or Visual Studio code.
3. Restore the NuGet packages by rebuilding the solution or run `dotnet restore`.
4. Build the project to ensure there are no compilation errors.
5. Run the project.

Optional CLI Commands:

```powershell
dotnet restore
dotnet build
```

## Blog Reference

* <a href="https://www.syncfusion.com/blogs/post/build-blazor-crud-application-with-dapper.aspx"> How to Build a Blazor CRUD Application with Dapper</a>
