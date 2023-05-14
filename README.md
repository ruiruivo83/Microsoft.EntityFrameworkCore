# Microsoft.EntityFrameworkCore
Sequence of commands in general

## 0 - Fiw connection String in appsettings.json
"Server=localhost;Database=DatabaseName;Trusted_Connection=True;Encrypt=true;TrustServerCertificate=true;"

## 1 - Create a migration after creating the models
Add-Migration "Migration Name"

## 2 - Apply migration script to database
Update-Database

## 3 - Scaffold from existing database to create Models
Scaffold-DbContext "Server=.\SQLExpress;Database=SchoolDB;Trusted_Connection=True;" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models


## 4 - If necessary - Replace existing Db_Context with new scaffolded DbContext

## 5 - Fix DbContext in Program.cs
