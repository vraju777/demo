# HackToHire Full Stack Project

A full-stack CRUD application built with **ASP.NET Core Web API**, **SQL Server**, and **Angular**.  
This project demonstrates backend API development, database integration, and a frontend UI for managing employees.

---

## 🚀 Tech Stack
- Backend: ASP.NET Core Web API (.NET 8)
- Database: SQL Server + Entity Framework Core
- Frontend: Angular 15
- Version Control: Git + GitHub

---

## 📂 Project Structure


---

## 🖥 Backend Setup
```bash
cd HackToHireApi
dotnet restore
dotnet ef migrations add InitialCreate
dotnet ef database update
dotnet run
## 🖥 sql setup Setup
CREATE DATABASE HackToHireDB;
CREATE LOGIN hackuser WITH PASSWORD = 'StrongPassword123!';
CREATE USER hackuser FOR LOGIN hackuser;
ALTER ROLE db_owner ADD MEMBER hackuser;

## 🖥 connection string Setup
"ConnectionStrings": {
  "DefaultConnection": "Server=localhost;Database=HackToHireDB;User Id=hackuser;Password=StrongPassword123!;"
}
## frentendstep
cd hack-to-hire-ui
npm install
ng serve -o
## github push
git init
git add .
git commit -m "Initial full stack project"
git branch -M main
git remote add origin https://github.com/vraju777/HackToHireFullStack.git
git push -u origin main
