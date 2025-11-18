# SQL-query Department
CREATE TABLE Department(
  EmpID INT IDENTITY(1,1) PRIMARY KEY,
  FiratName VARCHAR(50) NULL,
  LastName VARCHAR(50)NOT NULL,
  Email VARCHAR(120) UNIQUE,
  Gender CHAR(50) CHECK (gender in ('M','F')),
  Salary DECIMAL(10,2) DEFAULT 35000.00,
  DepartmentName VARCHAR(50),
  ProductName VARCHAR(100),
  SaledProduct VARCHAR(200),
  )
