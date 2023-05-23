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
</p>
<br />

<p>
 <a href="https://imgbox.com/90qME4ml" target="_blank"><img src="https://images2.imgbox.com/5b/31/90qME4ml_o.jpg" alt="image host"/></a>
</p>
Step 6: Download and Install C++ Redistributable following this link:
https://github.com/MicrosoftDocs/cpp-docs/blob/main/docs/windows/latest-supported-vc-redist.md
</p>
<br />

<p>
<a href="https://imgbox.com/HTsdJ94A" target="_blank"><img src="https://images2.imgbox.com/40/60/HTsdJ94A_o.jpg" alt="image host"/></a>
</p>
Step 7: Download and install mysql using the following link:
https://dev.mysql.com/downloads/installer/. Set up a username and password.
<p>
<br />
  
<p>
<a href="https://imgbox.com/P8w1Pqqu" target="_blank"><img src="https://images2.imgbox.com/ec/da/P8w1Pqqu_o.jpg" alt="image host"/></a>
</p>
Step 8: Click start and then type IIS, right click and then click "run as administrator". Double click php manager and register new php version, open and link to  C:php/php-cgi. When finished, single click on server and under manage server, restart the server.
<p>
<br />
  
<p>
<a href="https://imgbox.com/kd1bjZ9W" target="_blank"><img src="https://images2.imgbox.com/7e/a7/kd1bjZ9W_o.jpg" alt="image host"/></a>
</p>
Step 9: Download and Install OSticket using the following link:
https://osticket.com/download/. After download, navigate to the upload folder and drag and drop it into C:inetpub/wwwroot. After the upload folder is finished dropping, rename the upload folder to "osticket". Open IIS as administrator and restart server again.
<p>
<br />
<a href="https://imgbox.com/V8IFc9Ul" target="_blank"><img src="https://images2.imgbox.com/c2/90/V8IFc9Ul_o.jpg" alt="image host"/></a>
</p>
Step 10: In IIS, on the left hand side, expand the server, expand sites, expand default, and click osticket. On the right, click "browse *80(http)". This should load a osticket page, thanking you for choosing osticket. This loading indicates you have installed osticket correctly.
<p>
<br />

<p>
<a href="https://imgbox.com/2tG9ngDr" target="_blank"><img src="https://images2.imgbox.com/c0/8b/2tG9ngDr_o.jpg" alt="image host"/></a>
</p>
Step 11: Note that some extentions are missing from the OSticket install indicted by the page you loaded from the previous step. Go back to IIS, clicking sites -> Default --> OSticket, double click PHP manager. Enable the following extentions: php_imap.dll, php_intl.dll, and php_opcache.dll. Then refresh the osticket page you loaded in step 10 to see changes.
<p>
<br />
  
<p>
<a href="https://imgbox.com/mFp9Q7bf" target="_blank"><img src="https://images2.imgbox.com/08/d5/mFp9Q7bf_o.jpg" alt="image host"/></a>
</p>
Step 12: We need to give permission from everyone to use ost-config.php. Right click on ost-config and click on properties and then advanced. Click Disable inheritance, remove all permission. Then click add permissions, click principal and under "enter object name", type "everyone" and click "ok". Then checkmark "everyone" and press ok.
<p>
<br />

<p>
<a href="https://imgbox.com/aiSMJi5u" target="_blank"><img src="https://images2.imgbox.com/26/41/aiSMJi5u_o.jpg" alt="image host"/></a>
</p>
Step 13: Continue the osticket install by clicking continue on the previously loaded webpage and type in your name and default email. Fill in your admin information. Before we continue filling in the osticket page, we must set up Heidisql beforehand.
<p>
<br />
  
<p>
<a href="https://imgbox.com/EaNuqvHS" target="_blank"><img src="https://images2.imgbox.com/77/35/EaNuqvHS_o.jpg" alt="image host"/></a>
</p>
Step 14: Download and Install Heidisql using this link, https://www.heidisql.com/download.php, launch Heidisql and click new in the bottom left corner, use the password you used when installing mysql. Create a new database called osticket by right clicking "unnamed" and scroll to new and click "database". Go back to the osticket page and type into the database section the databse information you just created and click "install now" in the osticket webpage. After install it should load a congratulations page. This means OSticket loaded onto the server you just created successfully.
<p>
<br />
  
<p>
<a href="https://imgbox.com/kJXwBq7x" target="_blank"><img src="https://images2.imgbox.com/a8/90/kJXwBq7x_o.jpg" alt="image host"/></a>
Step 15: Delete the setup folder under the directory, c:\inetpub\wwwroot\osticket\setup. Browse to C:\inetpub\wwwroot\osticket\include\ost-config.php, right click on ost-config.php, click properties, then security, then advanced, highlight everyone and edit. Uncheck every permission except "read" and "read and execute". Click save and ok.





