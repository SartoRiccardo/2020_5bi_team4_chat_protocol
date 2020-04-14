# System Requirements

## 1. Introduction

The PCTO management application allows users to view the companies that collaborate with the school and offers tutors a simpler way of managing, adding, removing or modifying them. This document will provide instructions for accessing the site, researching and modifying companies.

## 2.Setup HTTP Server

An internet connection, a web server and a database connection are required to make the application work. You can also use a hosting service to put the site on.
A platform consisting of HTTP server is XAMPP.

1. Download XAMPP
	+ Go to [this website](https://www.apachefriends.org/it/)
	+ Download the correct version

2. Activate XAMPP
	+ Run xampp-control.exe
	+ Click on "Start" on Apache and MySQL

## 3. Access Application code

Access to the internet and a repository on GitHub used to store the code are required. Login credentials are required. All the code is stored in a repo on GitHub. The local files, on the other hand, are stored in the `htdocs` folder generated by XAMPP.

## 4. Install on Simulator or Device

### 4.1 Required Components

A computer with a software that allows to run virtual machines, such as VirtualBox, is required. There must be a virtual machine that acts as a server (the case of an Ubuntu machine is discussed). A web server, for example Apache, is needed.

### 4.2 Save the page

The page must be contained in a folder, preferably in `var/www/pcto`.

## 5. System Maintenance

The user interface consists of a table for viewing companies, plus the login screen. Everything is implemented in multiple files, using only HTML and PHP.
There is a file for each section. There is a section for:

+ Managing the login
+ Checking and redirecting to the correct page
+ Logging in as a student
+ Logging in as a tutor
+ Viewing specific information
+ Editing companies
+ Managing the logout.

On first launch, the application displays the login screen. Once the user is logged in, the view switches to the company table, which is displayed in the center of the screen. There is also a search bar at the top of the page. The logout button is located on the right and destroys all of the data associated with the current session.

The connection to the database allows you to view the companies, their information and modify them, also changing the corresponding row.