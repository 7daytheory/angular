## Installing SQL Server
Search Install SQL Server and go to official installation site. Click "Developer" version (It's free). Once installation has started choose "custom" installation, next page click "installation" on the side bar and choose New SQL Server standalone installation or add features to current installation". A new window will pop up for the installation.

Click next, until you have options on what you want to install(Feature Selection tab). In this case we are installing just "Database Engine Services". When you get to Database Engine Configuration, choose mixed mode and enter your password. Click next and your installation will be complete.

## SQL Server Management Studio
<strong>Just the user interface for working with SQL Server Studio</stong>
Use the same installation as the SQL Server above and click "SQL Server Management Server" on the feature selection tab. Install this with all defaults.
You can find it under Microsoft SQL Server Management Studio - use a . for localhost

## Visual Studio
Run through installations with defaults, and eventually in the installer you can choose packages you want included(you can modify them later also). 
- ASP.NET web Development
- Net Desktop Development
- Net Core Development

### Other programs being used - default settings
- Postman
- Visual Studio Code
- node
- angular (npm install -g @angular/cli)

### Setting up DB with SQL Server Management Studio
 - Click on the main SQL Server
 - Click on "New Query" in the toolbar
- You can execute queries here
- ex: "Create Database dbName"

### Examples of Creating and adding to the database

Creating Department Table
<code>
create table dbo.Department (
DepartmentID int identity(1,1),
DepartmentName varchar(500)
)

select * from dbo.Department

insert into dbo.Department values 
('Support'),
('IT'),
('Developer')
</code>

Creating Employee Table
<code>
create table dbo.Employee (
EmployeeID int identity(1,1),
EmployeeName varchar(500),
Department varchar(500),
DateOfJoining date,
PhotoFileName varchar(500),
)

insert into dbo.Employee values 
	('Matt','Developer', '2020-01-01', 'photoMatt.jpg'),
	('Glenn', 'Support', '2021-01-01', 'photoGlenn.jpg'),
	('Michele', 'Support', '2019-01-01', 'photoMichele.jpg'),
	('Erin', 'IT', '2017-01-01', 'photoErin.jpg')

	select * from dbo.Employee
</code>


