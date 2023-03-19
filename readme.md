# Introduction
That is a data scraping tool for scraping data from globaldatabase.com.\
It is a C# console application.

# Packages
* Selenium.WebDriver 4.8.1
* Selenium.Support 4.8.1
* DotNetSeleniumExtras.WaitHelpers 3.11.0

# Execution

## Version 1:
Name of country is hard-coded as country assigned to me was definite. Changing country name will not change execution behaviour of the program. You may change it.\
Login credentials are hard-coded.\
SQL connection string is hard-coded.

You need to run program thorugh console by sending required arguments.\
The program takes 3 arguments from console. 
* 1st argument is minimum number of employees,
* 2nd argument is maximum number of employees,
* 3rd argument is starting region index. Region index is just 1 in default. It will be automatically changed for next iterations.

Once all regions are iterated for given minimum and maximum employee numbers, 
minimum number of employees will be decreased by one and it also will be set as maximum as well and region will start from beginning too.

## Version 2:
As I lost access to data source when i was developing 2nd version, this version may be called as beta edition.
However, it is very close to release version.

Name of country is hard-coded as country assigned to me was definite. Changing country name will not change execution behaviour of the program. You may change it.\
Login credentials are hard-coded too.\
SQL connection string is hard-coded.

You need to run program thorugh console by sending required arguments.\
The program takes 3 arguments from console. 
* 1st argument is the index of the list where minimum and maximum number of employees are stored as hard-coded.
* 2nd argument is 'null_date' in default. It will be automatically calculated and set for next iterations.
* 3rd argument is 'false' in default. It basically indicates either date interval or employee number will be changed in the new iteration. This will be handled automatically too.

List that holds minimum and maximum number of employees list must be defined by user manually. 
Making an generic one that would work any for country, would be possible too.

# Possible Improvements
Obviously there are many possible improvements.

First of all, moving hard-coded values to outside of program could be nice. So these values can be changed without need of re-compiling the code.

Speed of scraping can be optimized. It is not slow though, but I didnt have so much time to work on it.

To increase the speed, I have got an idea. We may find a way to click 'show phone' and 'show email' buttons like 10 by 10, instead of 1 by 1.

Refactoring and cleaning the code could be another need. I would do it, if I have not lost access to data source.
