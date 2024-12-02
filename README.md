<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Download (osTicket)
- Enable IIS/CGI
- PHP Manager
- Install mySQL 5.5.62
- IIS
- Install os
- Post Installation Configurationsw

<h2>Installation Steps</h2>

<p>
<img width="1710" alt="image" src="https://github.com/user-attachments/assets/13962119-6687-4207-8f3c-30405e313701">

</p>
<p>
**Install osTicket** To start the process of installing osTicket; I opened and copied the file onto the desktop at which point I unzipped it by extracting it into osTicket on the desktop. After this step; to continue with the lab; I enabled Internet Information services (IIS) so the computer could recognise itself as a wed server by ging into Control panel and enabling IIS along with CGI. The server is now recognizable and will give feedback with loop back (127.0.0.1)
</p>
<br />

<p>
<img width="1710" alt="44AA3F53-CCB7-4F85-AB91-91FBA41BDAFC" src="https://github.com/user-attachments/assets/758fce9b-7db2-4152-9c2e-46fd6f467f5f">

</p>
<p>
**Install PHP Manger/My SQL 5.5.62** From within the unzipped osTIcket folder Installed (PHP manager) the scripting language for the webpage and (My SQL 5.5.62) The database for admins and users that will be used for the lab.
</p>
<br />

<p>
<img width="1710" alt="953316F0-29FE-4030-86A0-2BCA3A5013B7" src="https://github.com/user-attachments/assets/0c4b7b83-aa16-4ba4-a75a-ac8f5e1bb7b9">

</p>
<p>
**osTicket Installation** To complete the final instalation of (osTicket) I Registered PHP from inside (IIS Admin) to make my created web server aware of the PHP; browsing to the newly available executable binary located inside of flolder housing PHP and modifications (Windows (C)). After completion I extracted zipped osTicket folder from inside osTicket folder previously placed on desketop into My PHP folder. There is now a new folder availible with 2 items available inside. 
<p>
<img width="1710" alt="5DA4C4C6-BC70-4093-8847-1C741C8A9BF0" src="https://github.com/user-attachments/assets/a3e8ec60-acca-4e31-928e-0ed6cd1fde62">

**osTicket Continued** I copied one of the items (upload folder) into into inetpub/root folder, renamed upload folder to osTick and from within (IIS Manager) browsed to osTicket. osTicket is now Installed.

**Post Install configuration**
- From within PHP Manager I enabled extensions PHP(imap,intl,opcache)
- Renamed ost-sampleconfig.ph to ost-config.php by way of (file explore/windows C:\inetpub\wwwroot\osTicket\include). 
- From withing newley renamed folder new permissions were assigned. I disabled inheritance, removing previous permissions and added (ALL) as the new setting.

continue to osTicket
![image](https://github.com/user-attachments/assets/3c2ca270-6bbe-4d85-8c03-d757535b5673)

The final steps for configuring osTicket for use is creating a database and establishing a connection between the database previously created and the one that will be created later. To connect to my database I downloaded (HeidiSQL) from within the osTicket instalation files preeviously placed on the desktop (New/root credentials) a connection to database is now established 

![image](https://github.com/user-attachments/assets/fc9db933-a92d-4428-94b9-618bdedd7a30)

**Create osTicket Database**
Right click the unnamed (create new/database/name it osTicket). Now that the database is created I went back to database settings in the osTicket browser and plugged in newly created database and (root) credentials (osTicket/root/root).

osTicket is now installed and ready to use

![image](https://github.com/user-attachments/assets/024c13d6-eaf9-40cc-beab-53fc437c93ac)


