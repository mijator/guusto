
README.txt 


//
// 
// 
// **************** GUUSTO SEARCH APP *******************
//
//
//

This package (Zip file) contains the following files: 

index.html - this file is the login page
retrieve.jsp - this file is the search page
guustoServlet.java - this file handles the get/post variables
guusto.sql - this file sets up the database 
guusto.png - Guusto logo file
README.txt - this page showing the instructions

Once you have a PHP/MySQL webserver online or on a local machine 
using MAMP (free) or some other php/MySQL environment (e.g. cloud), 
you simply run the enclosed text file called guusto.sql as a MySQL import SQL, 
using phpMyAdmin or other admin. 

1. Here is what guusto.sql does: 

- creates a new database called guusto with 3 tables called data, region and merchant. 
- populates region with values for Canada and the U.S.A. 
- populates merchant with a few merchants 
- populates data table with region_id + merchant_id for each merchant

2. Install Local Webserver (e.g. apache)

Then you need to use a web browser to talk to the root server index.html webpage 
like this: 

http://localhost:80/GuustoSearch/index.html 

3. Login using the following credentials : 

username: jrota 
password: test 

4. You should now be logged into /GuustoSearch/retrieve.jsp which displays all of the merchants and regions 
and allows for sorting of the two parameters (i.e. region, merchant name). 



Known Bugs/Issues: 

- variables (i.e. username, password, flag) are being sent to the server but not being interpreted 
so that the sorting function does not work. This seems to be a server mis-configuration issue since 
the guustoServlet.java that handles DO_GET() and DO_POST() exists in the file called servlet.java. 



