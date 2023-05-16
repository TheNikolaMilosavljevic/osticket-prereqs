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

- Enabled Internet Information Services (IIS)
- Installed web platform installer
- Installed mysql, set up username and password
- Installed C++ redistributable

<h2>Installation Steps</h2>

<p>
<a href="https://imgbox.com/cEmIPWQl" target="_blank"><img src="https://thumbs2.imgbox.com/52/6d/cEmIPWQl_t.jpg" alt="image host"/></a>
</p>
<p>
Step 1: The first prerequisite is enabling Internet Information Services in order to run OSticket. Proceed to control panel and click on programs. Under programs. click enable services on/off and scroll down to IIS. Click "Internet Information Services" and make sure the box fills in. Then expand it by clicking on the "+" and look for "World Wide Web" and expand that. Then expand "Application Developer" and check "CGI".
</p>
<br />

<p>
<a href="https://imgbox.com/tNtAGPlz" target="_blank"><img src="https://thumbs2.imgbox.com/e0/4c/tNtAGPlz_t.jpg" alt="image host"/></a>
</p>
<p>
Step 2: Test whether or not you did step 1 correctly by opening your browser and typing "127.0.0.1" and clicking enter. The Internet Information Services web page should load and should look like the photo above.
</p>
<br /> 

<p>
<a href="https://imgbox.com/KtnSs9wo" target="_blank"><img src="https://images2.imgbox.com/a0/a9/KtnSs9wo_o.jpg" alt="image host"/></a>
</p>
<p>
Step 3: Install PHP manager for IIS by downloading the file using this link https://www.iis.net/downloads/community/2018/05/php-manager-150-for-iis-10 and install. 
</p>
<br />

<p>
<a href="https://imgbox.com/NLG5nFFC" target="_blank"><img src="https://images2.imgbox.com/4d/f0/NLG5nFFC_o.jpg" alt="image host"/></a>
</p>
<p>
Step 4: Download and Install Rewrite module using this link: https://www.iis.net/downloads/microsoft/url-rewrite
</p>
<br />

<p>
<a href="https://imgbox.com/zEU3qanN" target="_blank"><img src="https://images2.imgbox.com/95/dd/zEU3qanN_o.jpg" alt="image host"/></a>
  </p>
  <p>
Step 5: Create a new folder on your C: drive called PHP and download and extract this file into the newly created folder. Download link for PHP for windows: https://www.php.net/downloads.php
  
