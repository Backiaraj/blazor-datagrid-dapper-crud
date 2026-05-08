# Blazor DataGrid CRUD Application

A comprehensive example demonstrating how to build a full-stack Blazor CRUD application with real-time datagrid operations using [Dapper](https://github.com/DapperLib/Dapper) ORM and SQL Server. This repository contains multiple implementations across different .NET versions.

## Overview

This project showcases best practices for building interactive data management applications in Blazor with:

- **Server-side CRUD operations** against a SQL Server database
- **Real-time datagrid** with sorting, filtering, and inline editing
- **Type-safe data access** using Dapper ORM
- **Multiple framework versions** supporting .NET 5, .NET 6, and .NET 8

### Features

- **CRUD Operations** - Create, Read, Update, and Delete bug records
- **DataGrid** - Interactive table with real-time updates
- **Type-Safe Data Access** - Dapper with strongly-typed entities
- **Responsive UI** - Bootstrap-based responsive design
- **Data Validation** - Server-side validation for data integrity

## Prerequisites

- [.NET SDK 5.0](https://dotnet.microsoft.com/download/dotnet/5.0) or [.NET SDK 6.0](https://dotnet.microsoft.com/download/dotnet/6.0) or [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0) or later
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or later
- [Visual Studio Code](https://code.visualstudio.com/)
- **SQL Server** 2016 or later (Express edition supported)

### Setup Instructions

1. **Clone the repository**

   ```bash
   git clone https://github.com/SyncfusionExamples/blazor-datagrid-dapper-crud.git
   cd blazor-datagrid-dapper-crud
   ```

2. **Create the database**

   - Open SQL Server Management Studio (or your preferred SQL client)
   - Execute the script in `SQL Script/bug-table.sql` to create the **BugTracker** database and **Bugs** table
   
   Alternatively, use PowerShell:
   ```powershell
   sqlcmd -S <ServerName> -i "SQL Script\bug-table.sql"
   ```

3. **Configure the connection string**

   Edit the connection string in `appsettings.json` under the `BugTrackerDatabase` property:
   ```json
   {
     "ConnectionStrings": {
       "BugTrackerDatabase": "Server=<YOUR_SERVER>;Database=BugTracker;Trusted_Connection=true;Encrypt=false;"
     }
   }
   ```
   > Replace `<YOUR_SERVER>` with your SQL Server instance name (e.g., `localhost` or `.`)

4. **Restore and run**

   Choose your preferred project version:

   **BlazorWebApp (.NET 8 - Recommended)**
   ```bash
   cd BlazorWebApp
   dotnet restore
   dotnet build
   dotnet run
   ```

   **NET6 Version**
   ```bash
   cd NET6/Dapper.CRUD
   dotnet restore
   dotnet build
   dotnet run
   ```

   **NET5 Version**
   ```bash
   cd NET5/Dapper.CRUD
   dotnet restore
   dotnet build
   dotnet run
   ```


## Resources

- [Dapper GitHub Repository](https://github.com/DapperLib/Dapper)
- [SQL Server Documentation](https://learn.microsoft.com/en-us/sql/sql-server)
- [Blog: Build a Blazor CRUD Application with Dapper](https://www.syncfusion.com/blogs/post/build-blazor-crud-application-with-dapper.aspx)
