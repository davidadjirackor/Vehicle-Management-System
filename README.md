# Vehicle-Management-System (Fleet)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
[![APEX App](https://cdn.rawgit.com/Dani3lSun/apex-github-badges/b7e95341/badges/apex-app-badge.svg)](<LINK>)
[![APEX PL/SQL](https://cdn.rawgit.com/Dani3lSun/apex-github-badges/6ed914a1/badges/apex-plsql-badge.svg)](<LINK>)
[![APEX Built with Love](https://cdn.rawgit.com/Dani3lSun/apex-github-badges/7919f913/badges/apex-love-badge.svg)](<LINK>)
[![APEX Community](https://cdn.rawgit.com/Dani3lSun/apex-github-badges/78c5adbe/badges/apex-community-badge.svg)](<LINK>)

A system used to manage Fleet of vehicles migrated from Oracle Forms 6 to Oracle Application Express 18.1 - 22.1 

Link : https://g163858f7227eb0-pbj5dxgdsbwntfay.adb.ap-seoul-1.oraclecloudapps.com/ords/f?p=101:LOGIN_DESKTOP:12161845380396:::::

This repository contains two sql scripts 
 - vehicle_mamagement_database.sql contains the schema for the system. It has some dummy data. This can be truncated by users at will.(Did not want to disable constraints -reason i left the data in the tables)
 - Vehicle_management_apex_UI.sql contains the import of the Oracle Apex which is the UI of the application. This script contains supporting plugins [![APEX Plugin](https://cdn.rawgit.com/Dani3lSun/apex-github-badges/b7e95341/badges/apex-plugin-badge.svg)](<LINK>)  that have to be installed during the import process.


Usage 
-Create schema and import the vehicle_mamagement_database.sql script into it. 
-Import apex script into your oracle apex 22.1  
 installation build and run.  
 
Troubleshooting: 
There is a possiblity you wont be able to access the app after a successful import. 
If that happens: 
- Goto the application in Apex and click on <b>Shared Components</b>
- Under the Security Section click on Application Access Control 
- Click on Add User Role Assignment 
- A dialog box will open.Enter the user you want to add and checkbox their Role 
- Click on Create Assignment 
- Go back to the pages section select the Login Page (ususally 9999)  and run it. 
- You should be able to login now. 

![Capture](https://user-images.githubusercontent.com/13521226/182984028-e9576f17-6b76-4fde-818e-9ab82a615191.PNG)
