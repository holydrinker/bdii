## Web app for Database Systems II project
### Master Degree in Computer Science @ University of Bari

#### Required
- maven
- python (or other tool to run client)


#### Import Database
- Clone or download repository
- Create a postgres user (name: farmacista, password: farmacista)
- Find database/db.sql
- Open Postgres shell
- Import db typing `\i 'path/db.sql'`


#### Run application
- Clone or download repository
- Go with terminal into bdii-server directory and type `mvn exec:java -Dexec.mainClass="Server"`to run the server
- Go with terminal into bdii-client/app directory and type `python -mSimpleHTTPServer`to run the client
- Open your browser: http://localhost:8000/
- Enjoy


#### Navigate datawarehouse
- Download and install Apache Tomcat 7
- Download and extract Mondrian directory from here (http://www.di.uniba.it/~ceci/micFiles/courses/bdii/2011-2012/Lab/b-foodmart%20e%20mondrian.zip)
- Copy Mondrian directory into Tomcat/webapps
- Go into my directory database/dw and copy farmacia.xml and farmacia.jsp into Tomcat/webapps/mondrian/WEB-INF/queries
- Run tomcat (default port 8080)
- Open your browser: http://localhost:8080/mondrian/testpage.jsp?query=farmacia
- Enjoy


#### Sync datawarehouse
- While server is running, open your browser and type http://localhost:4567/dwSync
