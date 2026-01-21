# TODO List for JSP Servlet JDBC MySQL CRUD Example

## Completed Tasks
- [x] Create project directory 'jsp-servlet-jdbc-mysql-example'
- [x] Create subdirectories: src/, WebContent/, WebContent/WEB-INF/, WebContent/WEB-INF/lib/
- [x] Create User.java (JavaBean) at src/net/javaguides/usermanagement/model/User.java
- [x] Create UserDAO.java (DAO class) at src/net/javaguides/usermanagement/dao/UserDAO.java
- [x] Create UserServlet.java (controller servlet) at src/net/javaguides/usermanagement/web/UserServlet.java
- [x] Create user-list.jsp (list users page) at WebContent/user-list.jsp
- [x] Create user-form.jsp (add/edit form page) at WebContent/user-form.jsp
- [x] Create Error.jsp (error page) at WebContent/Error.jsp
- [x] Create db-setup.sql (database setup script) at root
- [x] Create web.xml (servlet configuration) at WebContent/WEB-INF/web.xml

## Pending Tasks
- [ ] Manually add required JAR files to WebContent/WEB-INF/lib/:
  - jsp-api-2.3.1.jar
  - servlet-api-2.3.jar
  - mysql-connector-java-8.0.13.jar
  - jstl-1.2.jar
- [ ] Set up MySQL database:
  - Run the db-setup.sql script to create 'demo' database and 'users' table
  - Ensure MySQL is running and adjust DB credentials in UserDAO.java if needed (default: root/root)
- [ ] Deploy the project:
  - Import into Eclipse as Dynamic Web Project or manually deploy WAR to Tomcat 8.5
  - Start Tomcat server
- [ ] Test the application:
  - Access at http://localhost:8080/jsp-servlet-jdbc-mysql-example/
  - Test CRUD operations: Create, Read, Update, Delete users
