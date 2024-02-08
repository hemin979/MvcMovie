					    [ CYB206: WEB APPLICATION SECURITY ]

			>=====================> ASP.NET Core MVC <=======================< 
						     ____________________________
							|Hemn Hamad Ameen - W0847826 |
							 ----------------------------

====> PART 1: Get started with ASP.NET Core MVC <====
 
2024-01-11 Created new project named "MvcMovie", having three folders: Controllers, Models and Views
Created the first web screen runnig this URL: https://localhost:7078/ --> showing a simple message "Welcome"
Added a picture with some a message. Now, the page has a new view 
 
====> PART 2: Add a controller <====

2024-01-18 Added a controller under Controller folder named "HelloWorldController" and updated with a some code.
Now the page URL is like this: https://localhost:7078/helloworld --> showing this message "This is my default action..."
The "HelloWorldController" controller updated with added code. Running the URL: https://localhost:7078/helloworld/welcome --> shwoing a different message "This is the Welcome action method..."
Done more updates to the welcome in the controller. Running the App to browse https://localhost:7078/helloworld/welcome?name=Hemin&numtimes=4. Now shows a different message "Hello Hemin, NumTimes is: 4 (this numerical value can be changed and message updates itself)

====> PART 3: Add a View <====

2024-01-20 Created a new forlder named "HelloWorld", adding a Razor "Index.cshtml" to the folder and replacing the code with some new code. 
Now, when running App to browse https://localhost:7078/helloworld, it shows a different message " Index.. Hello from our View Template!"
Updating parts of the controller "" code and now browsing https://localhost:7078/helloworld, showing a new message "My Movie List .. Hello from our View Template!"
Created a loop in the Welcome.cshtml view template that displays "Hello" NumTimes, replacing the code with new code. the final message is: "Welcome" some bullets with Hellow Hemin" that can be changed in the broweser.

====> PART 4: Add a Model <====

2024-01-25 Added a class under Model forlder and named "Movie.cs"
Added New Scaffolded Item under Controller forlder name "MovieController", adding SQL Server as database provider.
Now, coming to an important stage ----> "Migration", here is how it's done:
From the Tools menu, select NuGet Package Manager > Package Manager Console, then running these commands in the powershell: Add-Migration InitialCreate & Update-Databas

====> PART 5: work with a database in an ASP.NET Core MVC app <====

Examining the database: View Designer & View Data >> brwosing Movie.cs content in the database
Seed the database by creating "SeedData" under Models folder and updating the code. 
Add the seed initializer: Replacing the contents of Program.cs with new generated code.
Running App brwosing https://localhost:7078/Movies >> shows a table of all the movies stored in the database

====> PART 6: Controller Methods and Views in ASP.NET Core <====

2024-01-27 tested the app by editing the movie records (edit, create and delete) movies.
reviewed the code as per the tutorial
Updating the Models/Movie.cs file and add the highlighted lines

====> PART 7: add search to an ASP.NET Core MVC app <====

2024-01-27
Update the Index method found inside Controllers/MoviesController.cs with the some code
Update the Views/Movies/Index.cshtml file, and add the <form> Filter text box to the page

====> PART 8: Add a New Field to an ASP.NET Core MVC app <====
2024-02-08 12:40

Adding a "Rating" property to Models/Movie.cs module
Edit the /Views/Movies/Index.cshtml file and add a Rating field
Update the /Views/Movies/Create.cshtml with a Rating field
Update the SeedData, adding "Rating" to each record
Running Migration, build done
Database has been updated..


====> PART 9: Add a Validation an ASP.NET Core MVC app <====
2024-02-08 13:00

Update the Movie class to take advantage of the built-in validation attributes Required, StringLength, RegularExpression, Range and the DataType
disabled JavaScript in the Chrome browser

====> PART 10: Examine the Details and Delete Methods of an ASP.NET Core App <====
2024-02-08 13:20
Examined the Details method.
Examine the Delete and DeleteConfirmed methods

&&&&&&& Finally saving the updates to GitHub repository &&&&&&&

My Observations:

- It's been a fantastic experience, building an App drom scratch with Visual Studio.
- I have faced lots of difficulties, errors, the db was not populating. Fortunately, troubleshooted all the errors. 
