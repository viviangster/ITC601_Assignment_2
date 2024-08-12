you need to start xampp specifically mysql and apache
<br>go to phpmyadmin and make sure there is a database named "login_system"
<br>run the following sql command to create the appropriate table:
<br>CREATE TABLE password_resets (id INT AUTO_INCREMENT PRIMARY KEY, email VARCHAR(255) NOT NULL, token VARCHAR(255) NOT NULL, created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP);
<br>then run "node server.js" from the root directory of the project
<br>then go to phpmyadmin and localhost:3000
<br>can run "node newhash.js" to generate a new password hash
