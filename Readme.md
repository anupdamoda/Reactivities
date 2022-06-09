###### API Projects - Backend ######

# Command to create the solution
dotnet new sln

# Command to add a web api project under API folder - this creates a web api project
dotnet new webapi -n API

# Command to create the project under the respective folders
dotnet new classlib -n Application
dotnet new classlib -n Domain
dotnet new classlib -n Persistence

# Command to add the projects under the solution which is under the same folder
dotnet sln add API/API.csproj
dotnet sln add Application
dotnet sln add Domain
dotnet sln add Persistence

# Command to check the list the project under the solution
dotnet sln list

# Command to add reference of the difference projects
cd API
dotnet add reference ../Application
cd Application
dotnet add reference ../Domain
cd Persistence
dotnet add

# command to run the api project
dotnet run

# command to run the api project and automatically run if there are any other changes
dotnet watch run 

# in API Project - create the API controller 
which should return the api details back

# In Domain Project 
Create the Activity Class
Create the props (properties) in this Class
type Prop and then {Tab} 

# In order to search a file in the solution 
{Ctrl}+G

# Entity framework - in persistence project
go to Nuget Package Manager: press {Ctrl}+{Shift}+P
search for Nuget - if its not appearing add the visual studio code extension as 'Nuget Package Manager'
search for Nuget Add Package
Search for Package: Microsoft.EntityFrameworkCore.Sqlite
add into the Persistence project
