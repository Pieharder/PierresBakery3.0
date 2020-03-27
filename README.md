# _Pierre's Sweet and Savory Treats_

#### _Epicodus 2020 C#/React Cohort Advanced Database & Authentication Friday Project._

#### By _**Geoff Goetz | 27 March 2020**_

## Description

This program will allow (a) user(s) to signup, login, and logout. As well as add, update or delete savory treats. Only logged in users are able to add, edit and delete the savory treats or flavors, but any user can view all treats and flavors.

## Specifications:

| Behavior | Example Input | Example Output |
|:--------|:-------------:|:--------------:|
| Application does not allow a user to add Treats or Flavors if they are not logged in |Click: Flavor | "Log in with your account" |
| Application allows user to view Treats and Flavors when they are not logged in to the site | Click: Treats or Flavors | Treat or Flavor Details |
| Application allows user to create an account | Register | Login |
| Application allows user to login in to the site | Login | Welcome "User Name."|
| Application allows a logged in user to add a Treat to the database | Add Treat | Create Treat Page |
| Application allows a logged in user to add a Flavor to the database and asign a Treat | Add Flavor | Create Flavor Page |
| Application allows a logged in user to Edit a specific Treat | Edit Treat | Edit This Treat Form |
| Application allows a logged in user to Edit a specific Treat | Edit Treat | Edit This Treat Form |
| Application allows a logged in user to Edit a specific Flavor | Edit Treat | Edit This Treat Form |
| Application allows a logged in user to Delete a specific Treat | Delete | Are you sure you want to delete this Treat? |
| Application allows a logged in user to Delete a specific Flavor | Delete | Are you sure you want to delete this Flavor? |
| Application allows a user to Sign Out of the application | Log Out | Please Sign Up or Login | 

## Setup/Installation Requirements

### Install .NET Core

#### on macOS:
* _[Click here](https://dotnet.microsoft.com/download/thank-you/dotnet-sdk-2.2.106-macos-x64-installer) to download a .NET Core SDK from Microsoft Corp._
* _Open the file (this will launch an installer which will walk you through installation steps. Use the default settings the installer suggests.)_

#### on Windows:
* _[Click here](https://dotnet.microsoft.com/download/thank-you/dotnet-sdk-2.2.203-windows-x64-installer) to download the 64-bit .NET Core SDK from Microsoft Corp._
* _Open the .exe file and follow the steps provided by the installer for your OS._

#### Install dotnet script
_Enter the command ``dotnet tool install -g dotnet-script`` in Terminal (macOS) or PowerShell (Windows)._

### Install MySQL and MySQL Workbench

#### on macOS:
_Download the MySQL Community Server DMG File [here](https://dev.mysql.com/downloads/file/?id=484914). Follow along with the installer until you reach the configuration page. Once you've reached Configuration, set the following options (or user default if not specified):_
* use legacy password encryption
* set password (and change the password field in appsettings.json file of this repository to match your password)
* click finish
* open Terminal and enter the command ``echo 'export PATH="/usr/local/mysql/bin:$PATH"' >> ~/.bash_profile`` if using Git Bash.
* Verify MySQL installation by opening Terminal and entering the command ``mysql -uroot -p{your password here, omitted brackets}``. If you gain access to the MySQL command line, installation is complete. An error (e.g., -bash: mysql: command not found) indicates something went wrong.

_Download MySQL Workbench DMG file [here](https://dev.mysql.com/downloads/file/?id=484391). Install MySQL Workbench to Applications folder. Open MySQL Workbench and select Local instance 3306 server, then enter the password you set. If it connects, you're all set._

#### on Windows:
_Download the MySQL Web Installer [here](https://dev.mysql.com/downloads/file/?id=484919) and follow along with the installer. Click "Yes" if prompted to update, and accept license terms._
* Choose Custom setup type
* When prompted to Select Products and Features, choose the following: MySQL Server (Will be under MySQL Servers) and MySQL Workbench (Will be under Applications)
* Select Next, then Execute. Wait for download and installation (can take a few minutes)
* Advance through Configuration as follows:
  - High Availability set to Standalone.
  - Defaults are OK under Type and Networking.
  - Authentication Method set to Use Legacy Authentication Method.
  - Set password to epicodus. You can use your own if you want but epicodus will be assumed in the lessons.
  - Unselect Configure MySQL Server as a Windows Service.
* Complete installation process

_Add the MySQL environment variable to the System PATH. Instructions for Windows 10:_
* Open the Control Panel and visit _System > Advanced System Settings > Environment Variables..._
* Select _PATH..._, click _Edit..._, then _Add_.
* Add the exact location of your MySQL installation and click _OK_. (This location is likely C:\Program Files\MySQL\MySQL Server 8.0\bin, but may differ depending on your specific installation.)
* Verify installation by opening Windows PowerShell and entering the command ``mysql -uroot -p{your password here, omitted brackets}``. It's working correctly if you gain access to the MySQL command line. Exit MySQL by entering the command ``exit``.
* Open MySQL Workbench and select Local instance 3306 server (may be named differently). Enter the password you set, and if it connects, you're all set.

### Clone this repository

_Enter the following commands in Terminal (macOS) or PowerShell (Windows):_
* ``cd desktop``
* ``git clone https://github.com/Pieharder/PierresBakery3.0``
* ``cd PierresBakery3.0``

_Confirm that you have navigated to the HairSalon.Solution directory (e.g., by entering the command_ ``pwd`` _in Terminal)._

_Change into the working directory of the project:_
* ``cd PierresBakery``

_Run the migration command to populate your MySQL server with the Database and Tables associated with this project:_
* ``dotnet ef database update``

_Run this application by entering the following command in Terminal (macOS) or PowerShell (Windows):_
* ``cd PierresBakery3.0``
* ``cd PierresBakery``
* ``dotnet restore``
* ``dotnet build``
* ``dotnet run`` or ``dotnet watch run``

_To view/edit the source code of this application, open the contents of the ``PierresBakery3.0`` directory in a text editor or IDE of your choice (e.g., to open all contents of the directory in Visual Studio Code on macOS, enter the command_ ``code .`` _in Terminal)._

## Technologies Used
* _Git_
* _HTML_
* _CSS_
* _C#_
* _.NET Core 2.2_
* _ASP.NET Core MVC (version 2.2)_
* _Razor_
* _dotnet script_
* _MySQL 8.0 CE_
* _MySQL Workbench 8.0 CE_
* _Entity Framework Core 2.2_
* _Michelle M README Template_

### License

*This webpage is licensed under the MIT license.*

Copyright (c) 2020 **_Geoff Goetz_**