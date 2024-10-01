# 3-tier-app-using-docker-docker-compose


   DEPLOY THREE TIER APPLICATION USING DOCKER AND DOCKER COMPOSE.


TYPES OF ARCHITECTURES
•	ONE-TIER 
•	TWO-TIER 
•	THREE-TIER N-TIER

 

 
 ![image](https://github.com/user-attachments/assets/4eb14c2b-62cd-4866-9662-276ed0d9cb3a)


![image](https://github.com/user-attachments/assets/1de8c00a-41b7-4b8a-9133-25938d0fa685)

![image](https://github.com/user-attachments/assets/42ee2ec6-7728-437a-a6bd-cc771023fbb9)

![image](https://github.com/user-attachments/assets/f7226e82-02f4-45ad-8de4-881973c26072)
 
![image](https://github.com/user-attachments/assets/1703465a-f768-4ffd-9ead-c403c413604d)
 
![image](https://github.com/user-attachments/assets/7e3e4588-dbd1-4dbc-86e4-5c3fcb37b8d0)
 
![image](https://github.com/user-attachments/assets/afc5e44f-121e-4cf7-a478-8a1d86cfb178)
 
![image](https://github.com/user-attachments/assets/d9275c8a-f6af-4214-9171-ed3688bbc908)
 
![image](https://github.com/user-attachments/assets/9cb48556-e389-4676-8500-e2ea496a2c2e)
 
![image](https://github.com/user-attachments/assets/0576541c-8c53-4a68-a93b-e7bb0813f610)
 

WHAT IS THREE TIER APPLICATION?

 

•	In software development, it’s very common to see applications built with a specific architectural paradigm in mind. 
•	One of the most prevalent patterns seen in modern software architecture is the 3-tier (or three-tier) architecture.
•	This model structures an application into three distinct tiers: presentation (user interface), logic(business logic), and data (data storage).
•	The fundamental advantage of 3-tier architecture lies in the clear separation of concerns.
•	Each tier operates independently, allowing developers to focus on specific aspects of the application without affecting other layers.
•	This enhances maintainability, as updates or changes can be made to a single tier with minimal impact on the others. 
•	3-tier applications are also highly scalable since each tier can be scaled horizontally or vertically to handle increased demand as usage grows.
A 3-tier application is a model that divides an application into three interconnected layers:
•	Presentation Tier: The user interface where the end-user interacts with the system (e.g., a web browser or a mobile app).
•	Logic Tier: The middle tier of the architecture, also known as the logic tier, handles the application’s core processing, business rules, and calculations.
•	Data Tier: Manages the storage, retrieval, and manipulation of the application’s data, typically utilizing a database.
This layered separation offers several key advantages that we will explore in more depth later in the post, but first, let’s examine them at a high level. 
First, it allows for scalability since each tier can be scaled independently to meet changing performance demands. Second, 3-tier applications are highly flexible; tiers can be updated or replaced with newer technologies without disrupting the entire application. Third, maintainability is enhanced, as modifications to one tier often have minimal or no effect on other tiers. Finally, a layered architecture allows for improved security, as multiple layers of protection can be implemented to safeguard sensitive data and business logic.


How does a 3-tier application architecture work?
The fundamental principle of a 3-tier application is the flow of information and requests through the tiers. Depending on the technologies you use, each layer has mechanisms that allow each part of the architecture to communicate with the other adjacent layer. Here’s a simplified breakdown:

1.	User Interaction: The user interacts with the presentation tier (e.g., enters data into a web form or clicks a button on a mobile app).
2.	Request Processing: The presentation tier sends the user’s request to the application tier.
3.	Business Logic: The logic tier executes the relevant business logic, processes the data, and potentially interacts with the data tier to retrieve or store information.
4.	Data Access: If necessary, the application tier communicates with the data tier to access the database, either reading data to be processed or writing data for storage.
5.	Response: The logic tier formulates a response based on the processed data and business rules and packages it into the expected format the presentation tier requires.
6.	Display: The presentation tier receives the response from the application tier and displays the information to the user (e.g., updates a webpage or renders a result in a mobile app).
The important part is that the user never directly interacts with the logic or data tiers. All user interactions with the application occur through the presentation tier. The same goes for each adjacent layer in the 3-tier application. For example, the presentation layer communicates with the logic layer but never directly with the data layer. To understand how this compares to other n-tier architectural styles, let’s take a look at a brief comparison.
The logical tiers of a 3-tier application architecture
The three tiers at the heart of a 3-tier architecture are not simply physical divisions; they also represent a separation in technologies used. Let’s look at each tier in closer detail:
1. Presentation tier
•	Focus: User interaction and display of information.
•	Role: This is the interface that users see and interact with. It gathers input, formats and sanitizes data, and displays the results returned from the other tiers.
•	Technologies:
o	Web Development: HTML, CSS/SCSS/Sass, TypeScript/JavaScript, front-end frameworks (React, Angular, Vue.js), a web server.
o	Mobile Development: Platform-specific technologies (Swift, Kotlin, etc.).
o	Desktop Applications: Platform-specific UI libraries or third-party cross-platform development tools.
2. Logic tier
•	Focus: Core functionality and business logic.
•	Role: This tier is the brain of the application. It processes data, implements business rules and logic, further validates input, and coordinates interactions between the presentation and data tiers.
•	Technologies:
o	Programming Languages: Java, Python, JavaScript, C#, Ruby, etc.
o	Web Frameworks: Spring, Django, Ruby on Rails, etc.
o	App Server/Web Server
3. Data tier
•	Focus: Persistent storage and management of data.
•	Role: This tier reliably stores the application’s data and handles all access requests. It protects data integrity and ensures consistency.
•	Technologies:
o	Database servers: Relational (MySQL, PostgreSQL, Microsoft SQL Server) or NoSQL (MongoDB, Cassandra).
o	Database Management Systems: Provide tools to create, access, and manage data.
o	Storage providers (AWS S3, Azure Blobs, etc)
Separating concerns among these tiers enhances the software’s modularity. This makes updating, maintaining, or replacing specific components easier without breaking the whole application.
3-tier application examples
Whether a desktop or web app, 3-tier applications come in many forms across almost every industry. Here are a few relatable examples of how a 3-tier architecture can be used and a breakdown of what each layer would be responsible for within the system.
E-commerce websites
•	Presentation Layer: The online storefront with product catalogs, shopping carts, and checkout interfaces.
•	Logic Layer: Handles searching, order processing, inventory management, interfacing with 3rd-party payment vendors, and business rules like discounts and promotions.
•	Data Layer: Stores product information, customer data, order history, and financial transactions in a database.
Online booking platforms (e.g., hotels, flights, appointments)
•	Presentation Layer: Search features, promotional materials, and reservation interfaces.
•	Logic Layer: Handles availability checks, real-time pricing, booking logic, and payment processing to 3rd-party payment vendors.
•	Data Layer: Stores schedules, reservations, inventory information, and customer details.
Of course, these are just a few simplified examples of a 3-tier architecture in action. Many of the applications we use daily will use a 3-tier architecture (or potentially more tiers for a modern web-based application), so finding further examples is generally not much of a stretch. The examples above demonstrate how application functionality can be divided into one of the three tiers.
Benefits of a 3-tier app architecture
One of the benefits of the 3-tier architecture is it’s usually quite apparent why using it would be advantageous over other options, such as a two-tier architecture. However, let’s briefly summarize the advantages and benefits for developers, architects, and end-users who will build or utilize the 3-tier architecture pattern.
Scalability
Each tier can be independently scaled to handle increased load or demand. For example, you can add more servers to the logic tier to improve processing capabilities without affecting the user experience or add more database servers to improve query performance.
Maintainability
Changes to one tier often have minimal impact on the others, making it easier to modify, update, or debug specific application components. As long as contracts between the layers (such as API definitions or data mappings) don’t change, developers can benefit from shorter development cycles and reduced risk.
Flexibility
You can upgrade or replace technologies within individual tiers without overhauling the entire system. This allows for greater adaptability as requirements evolve. For example, if the technology you are using within your data tier does not support a particular feature you need, you can replace that technology while leaving the application and presentation layers untouched, as long as contracts between the layers don’t change (just as above).
Improved Security
Multiple layers of security can be implemented across tiers. This also isolates the sensitive data layer behind the logic layer, reducing potential attack surfaces. For instance, you can have the logic layer enforce field-level validation on a form and sanitize the data that comes through. This allows for two checks on the data.
Reusability 
Components within the logic tier can sometimes be reused in other applications, promoting efficiency and code standardization. For example, a mobile application, a web application, and a desktop application may all leverage the same application layer and corresponding data layer. If the logic layer is exposed externally through a REST API or similar technology, it also opens up the possibility of leveraging this functionality for third-party developers to take advantage of the API and the underlying functionality.
Developer specialization 
Teams can specialize in specific tiers (e.g., front-end, back-end, database), optimizing their skills and improving development efficiency. Although many developers these days focus on full-stack development, larger organizations still divide teams based on frontend and backend technologies. Implementing a 3-tier architecture fits well with this paradigm of splitting up responsibilities.
The benefits listed above cover multiple angles, from staffing and infrastructure to security and beyond. The potential upside of leveraging 3-tier architectures is wide-reaching and broadly applicable. It leaves no question as to why 3-tier architectures have become the standard for almost all modern applications. That being said, many times, the current implementation of an application can be improved, and if an application is currently undergoing modernization, how do you ensure that it will meet your target and future state architecture roadmap? This is where vFunction can swoop in and help.


STEP 1:  Create A EC2 AMAZON LINUX INSTANCE.

![image](https://github.com/user-attachments/assets/f662d83b-bac1-408a-bdd7-e4a6ac0895db)
 

STEP 2: CONNECT TO EC2 INSTANCE.
INSTALL DOCKER:
                                    yum install docker -y
                                   systemctl start docker 
INSTALL GIT:
            
                          yum install git  -y
STEP 3: CLONE THE APPLICATION CODE TO EC2 SERVER
                         git clone repo-url
              git clone https://github.com/Praveenchoudary/ltibbhackathon.git

![image](https://github.com/user-attachments/assets/7f311519-9d96-4ebd-8293-9aa49a5ce58d)
 
STEP 4: GO TO THE DIRECTORY WHERE SOURCE CODE IS AVAILABLE.
                               cd ltibbhackathon/ 
 
![image](https://github.com/user-attachments/assets/cde145d9-a056-430c-84c4-9467fed1ab06)

STEP 5: WRITE DOCKER FILE FOR APPLICATION.
FROM php:7.4-apache  #apache base image
RUN docker-php-ext-install mysqli
COPY . /var/www/html/    #default path of webserver

![image](https://github.com/user-attachments/assets/d170af64-4037-466b-9657-616d91bd2bee)

 
STEP 6: Create a Folder backend and Write mysql file and  Docker file for DATABASE.
 ![image](https://github.com/user-attachments/assets/b5304ef3-4507-43eb-8e9a-55ee4686f1cd)
 

vim init.sql:
Create database customers;
use customers;
create table donors(id int AUTO_INCREMENT primary key, fname varchar(255) NOT NULL , lname varchar(255) NOT NULL , mobileno BIGINT UNIQUE, city varchar(255) NOT NULL, bfrom date, bto date, dob date, bloodgroup varchar(255) NOT NULL);
INSERT INTO donors (fname, lname, mobileno, city, bfrom, bto, dob, bloodgroup) VALUES ('Srikanth', 'Koraveni', '9000736060', 'Pune', '2022-09-28', '2022-12-28', '1998-05-22', 'O_Positive'), ('Prashanth', 'Katkam', '7989919097', 'Mumbai', '2022-09-17', '2022-11-18', '1998-09-30', 'O_Positive'), ('Kranthi', 'Khaitha', '9876789871', 'Bangalore', '2022-09-16', '2022-11-08', '1996-07-02', 'B_Positive'), ('Srinivas', 'Thota', '9812789411', 'Mumbai', '2022-09-18', '2022-10-31', '1992-07-22', 'O_Positive'), ('Pandya', 'Loka', '9877787887', 'Mumbai', '2022-09-18', '2022-10-09', '1992-07-22', 'B_Positive'), ('Prajodh', 'Shreya', '9812444411', 'Mumbai', '2022-08-23', '2022-10-31', '1992-07-22', 'B_Positive'), ('Srinivas', 'Thota', '9812723411', 'Mumbai', '2022-04-19', '2022-10-07', '1992-07-22', 'B_Positive'), ('Zaheer', 'Khan', '7788678987', 'Chennai', '2022-09-11', '2022-12-19', '1998-11-11', 'A_Positive');
CREATE TABLE users ( username varchar(80) NOT NULL, name varchar(80) NOT NULL, password varchar(80) NOT NULL ) ENGINE=InnoDB DEFAULT CHARSET=latin1;
INSERT INTO `users` (`username`, `name`, `password`) VALUES
('yssyogesh', 'Yogesh Singh', '12345'),
('bsonarika', 'Sonarika Bhadoria', '12345'),
('vishal', 'Vishal Sahu', '12345'),
('prashanth', 'Prashanth Katkam', '12345'),
('vijay', 'Vijay mourya', '12345');
INSERT INTO users (username, name, password) VALUES ('prashanth', 'Prashanth Katkam', '12345');
CREATE TABLE admin ( username varchar(80) NOT NULL, name varchar(80) NOT NULL, password varchar(80) NOT NULL ) ENGINE=InnoDB DEFAULT CHARSET=latin1;
INSERT INTO admin (username, name, password) VALUES ('admin', 'admin', '12345');
GRANT ALL PRIVILEGES ON customers.* TO 'root'@'%' IDENTIFIED BY 'admin123'; FLUSH PRIVILEGES;


 ![image](https://github.com/user-attachments/assets/fd28566c-380b-4df5-803b-fb19bd5c62e8)


vim Dockerfile (For Database)
FROM mysql/mysql-server:5.7
COPY . /init.sql /docker-entrypoint-initdb.d/
ENV MYSQL_ROOT_PASSWORD=admin123

 ![image](https://github.com/user-attachments/assets/3e698bc4-c8fc-4ec8-b34f-0571bd86363b)
               


STEP 7: Update .php file with server name as “mysqldb” and user as “root”

                             
 ![image](https://github.com/user-attachments/assets/0b51d92e-8e23-4d27-9eba-ebaf0d42f77f)
                        

STEP 8: BUILD DOCKER FILE TO CREATE DOCKER IMAGES FOR BOTH FRONTEND AND DATABASE.
                                        docker build -t myapp .
                                        docker build -t mydb backend
  


 ![image](https://github.com/user-attachments/assets/f78ee7ce-4560-4d11-ab6e-30de08ba6467)

![image](https://github.com/user-attachments/assets/66ce046b-bce4-4943-b20c-23d695558e2c)

•	Two docker images is created.
STEP 9: CREATE A CONTAINER FROM THE IMAGES. (FIRST CREATE CONTAINER FOR DATABASE)

                    docker run -d –name mysqldb -p 3306:3306 mydb


STEP 10: CREATE A CONTAINER FOR APPLICATION AND LINK TO DATABASE CONTAINER.
              docker  run -itd –name bloodbank -p 1234:80 –link myqldb:sqlconn myapp
 

![image](https://github.com/user-attachments/assets/1677baeb-5504-46b8-90cc-eb8c168109ab)

STEP 11: NOW ACCES THE APPLICATION USING PUBLIC IP OF EC2 INSTANCE WITH PORT NUMBER 1234
                 
![image](https://github.com/user-attachments/assets/c711f467-0b18-4d9c-badf-7298de553bc5)
 

STEP 12: NOW CREATE USER IN APP THROUGH SIGNUP AND CHECK WHETHER 
THE DATE IS -STORING IN DATABASE

![image](https://github.com/user-attachments/assets/f0263dc9-c7a2-42fa-917a-59d1473ae487)
 

•	CLICK ON DONATE BLOOD.
 

![image](https://github.com/user-attachments/assets/c11cf6f2-88c9-4140-9a7b-0bdd217e7181)




•	Login with user name and password
                 
![image](https://github.com/user-attachments/assets/c71f8a55-43f4-43d4-b091-7d61d57af471)

Fill the Donor Data.

![image](https://github.com/user-attachments/assets/8b913d87-e1d5-4297-b1ba-bee2a7057334)



![image](https://github.com/user-attachments/assets/178c661c-8c5c-4622-9bd0-e0330fd21e75)
 

CHECK THE DATA IS STORED IN DATABASE.

![image](https://github.com/user-attachments/assets/842f06b8-3d8b-4cec-9a67-95c4b5b8b68d)
 

CHECK THE DONOR DETAILS IN APPLICATION.BY CLICKING ON FIND DONOR
 


![image](https://github.com/user-attachments/assets/e59c3207-9d2b-4f7a-bbe6-66e0a5f7ee50)
 
![image](https://github.com/user-attachments/assets/9162f3cf-e68b-4c45-a13e-ea3f7a63ffdb)

STEP 13: PUSH THE IMAGE TO DOCKERHUB.
•	TAG THE IMAGES.

docker tag myapp praveen22233/bloodbank:appimage
docker tag myapp praveen22233/bloodbank:dbimage

 
![image](https://github.com/user-attachments/assets/1570f8e6-4dcd-412f-806c-aeb93eafc1e3)


•	LOGIN INTO DOCKER HUB 

         docker login > provide username and password of dockerhub.

![image](https://github.com/user-attachments/assets/ad2e0236-7056-4bc9-bf8e-839f647e62ab)
 

•	Push the images to docker using below command.
                         docker push praveen22233/bloodbank:appimage
                        docker push praveen22233/bloodbank:dbimage



         DEPLOY THE SAME APPLICATION USING DOCKER COMPOSE

STEP 1: INSTALL DOCKER COMPOSE.
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
ls /usr/local/bin/
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker-compose version

![image](https://github.com/user-attachments/assets/497afc88-b218-4d63-a8b1-be8e4edafcce)
 

STEP 2: WRITE DOCKER COMPOSE FILE
docker-compose.yml

---
version: "3"
services:
  db:
    container_name: mysqldb
    build: ./backend
    ports:
      - "3306:3306"
  app:
    container_name: bloodbank
    build: ./
    ports:
      - "1234:80"
    depends_on:
      - db

 
![image](https://github.com/user-attachments/assets/21fcc443-c383-4232-8d6c-6f4e97c03bfa)


 ![image](https://github.com/user-attachments/assets/a3a84808-aac7-43df-b98c-98a328c02a96)

•	ACCESS THE APPLICATION USING PUBLIC_IP OF EC2 INATANCE WITH PORT NUMBER.
                           http://3.82.153.117:1234/

 
![image](https://github.com/user-attachments/assets/97028175-8cf5-4061-bd1d-de68c4f629f0)

![image](https://github.com/user-attachments/assets/b6b7c32a-8661-4880-b44e-d7b27e860954)

