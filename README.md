Requirements:
1. PMS contains information about projects and tasks. Every task belongs to some project. Task can contain
subtasks and project can contain subprojects.
2. For every project following attributes are stored in PMS:
a. Code
b. Name
c. Start date
d. Finish date
e. State
3. For every task following attributes are stored in PMS:
a. Name
b. Description
c. Start date
d. Finish date
e. State
4. State of task is set when task is updated and can be one of the following values: Planned, inProgress, Completed
5. State of project is always calculated by the following rules:
a. Completed, if all tasks in the project and its subprojects have state Completed
b. inProgress, if there is at least one task with state inProgress in project or its subprojects
c. Planned in all other cases

The microservice must contain:
1. Database for storing information about tasks and projects, use MS SQL Server 2012+
2. Web API for CRUD operations, use ASP.NET MVC 5 or ASP.NET Core
3. Web API for retrieving report with list of all projects and tasks with state inProgress for some date in .xlsx format
(Excel 2007+), use ASP.NET MVC 5 or ASP.NET Core
You should prepare the code, unit tests and documentation as you would any piece of professionally written software.
The purpose of this exercise is to demonstrate your programming skills in an exercise that should not take more than a
few hours of your time. When you feel it is appropriate to use a library outside of the standard libraries, then please
notate that library declaration with a comment explaining motivation for use.
As we are also interested in your thought process and work method, when you submit the challenge, please zip together
the source control repository that you used so that we may inspect the commit history.
