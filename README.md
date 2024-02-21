# Workplace-Feb24
Project 24 Placement Intern  
<p>Databases

<p>Page Delete, edit, Create. 

![image](https://github.com/Dm2998/Workplace-/assets/114578666/66348a0e-1fea-4a73-a4b2-d0cfcdc738bf)


<br>
"
<p>-- Create Car table
  <br>
CREATE TABLE hi_Car (
  CarID int NOT NULL PRIMARY KEY,
  Model varchar(50) NOT NULL,
  Price decimal(18, 2) NOT NULL,
  Year int NOT NULL,
  Color varchar(20) NOT NULL,
  Quantity int NOT NULL,
  ImageFile  varbinary(MAX)
);

<p>-- Create Customer table
  <br>
CREATE TABLE hi_Customer (
  CustomerID int NOT NULL PRIMARY KEY,
  Name varchar(50) NOT NULL,
  Address varchar(100) NOT NULL,
  Email varchar(50) NOT NULL,
  Mobile_No varchar(15) NOT NULL
);

<p>-- Create Inquiries table
<br>
CREATE TABLE hi_Inquiry (
  InquiryID int NOT NULL PRIMARY KEY,
  CarID int NOT NULL,
  Message varchar(255) NOT NULL,
  CustomerID int NOT NULL,
  FOREIGN KEY (CarID) REFERENCES hello_Car(CarID),
  FOREIGN KEY (CustomerID) REFERENCES hello_Customer(CustomerID)
);

<p>-- Create Search table
  <br>
CREATE TABLE hi_Search (
  SearchID int NOT NULL PRIMARY KEY,
  CarModel varchar(50) NOT NULL,
  SearchDate date NOT NULL,
  CustomerID int NOT NULL,
  FOREIGN KEY (CustomerID) REFERENCES hello_Customer(CustomerID)
);

<>br-- Create Registration table
<br>
CREATE TABLE hi_Registration (
  RegistrationID int NOT NULL PRIMARY KEY,
  Firstname varchar(50) NOT NULL,
  Lastname varchar(50) NOT NULL,
  Email varchar(50) NOT NULL,
  Address varchar(100) NOT NULL,
  PhoneNumber varchar(15) NOT NULL
);





<p>-- Insert data into hello_Car table
<br>
INSERT INTO hello_Car (CarID, Model, Price, Year, Color, Quantity, ImageFile)
VALUES (1, 'Toyota Camry', 25000.00, 2022, 'Blue', 5, 'camry.jpg');

<p>-- Insert data into hello_Customer table
<br>
  INSERT INTO hello_Customer (CustomerID, Name, Address, Email, Mobile_No)
VALUES (1, 'John Doe', '123 Main St', 'john.doe@example.com', '123-456-7890');

<p>-- Insert data into hello_Inquiry table
<br>
INSERT INTO hello_Inquiry (InquiryID, CarID, Message, CustomerID)
VALUES (1, 1, 'I'm interested in the Toyota Camry.', 1);

<p>-- Insert data into hello_Search table
<br>
INSERT INTO hello_Search (SearchID, CarModel, SearchDate, CustomerID)
VALUES (1, 'Toyota Camry', '2024-02-15', 1);

<p>-- Insert data into hello_Registration table

  <br>
  INSERT INTO hello_Registration (RegistrationID, Firstname, Lastname, Email, Address, PhoneNumber)
VALUES (1, 'Jane', 'Doe', 'jane.doe@example.com', '456 Oak St', '987-654-3210');



<br>
<h1> package to Install

<br>
<p>Microsoft.AspNetCore.Identity.EntityFrameworkCore
<p>Microsoft.EntityFrameworkCore.Tools
<p>Microsoft.EntityFrameworkCore.SqlServer


<br>

![image](https://github.com/Dm2998/Workplace-/assets/114578666/6c98f9e1-aae5-43b5-94b6-49bba3cf69fa)

<br>

install Entity Framework Core in .NET. Entity Framework Core is an object-relational mapper (ORM) that enables you to work with relational databases using objects.

Here are the steps on how to get the packages listed in the image:

Open Visual Studio.
Click on New Project.
In the search bar, type in ASP.NET Core Web Application.
Select the ASP.NET Core Web Application template and click Next.
In the Name field, type in a name for your project.
Click Create.
In the Solution Explorer, right-click on your project and select Manage NuGet Packages.
In the search bar, type in Microsoft.EntityFrameworkCore.
Click on the Microsoft.EntityFrameworkCore package and click Install.
Repeat steps 8 and 9 for the following packages:
Microsoft.AspNetCore.Identity.EntityFrameworkCore
Microsoft.EntityFrameworkCore.Tools
Microsoft.EntityFrameworkCore.SqlServer
Once you have installed all of the packages, you will be able to use Entity Framework Core in your project.

Here are some additional resources that you may find helpful:

Microsoft documentation on Entity Framework Core: https://docs.microsoft.com/en-us/ef/core/
Entity Framework Core getting started guide: https://docs.microsoft.com/en-us/ef/core/get-started/
'
<br>
<br>

![image](https://github.com/Dm2998/Workplace-/assets/114578666/986c5171-c43d-4278-8e61-ffdebbfb0c0a)


<br>

Git repo


![image](https://github.com/Dm2998/Workplace-/assets/114578666/cfecc3fa-3eb0-49dd-b3bc-6a2c92a47ec7)





