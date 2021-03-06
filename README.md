# phpBB-3.x-API-Registration-Mod-Revisited


[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/shibdib/API-Registration-Mod-Revisited.svg)](http://isitmaintained.com/project/shibdib/API-Registration-Mod-Revisited "Average time to resolve an issue")  [![Percentage of issues still open](http://isitmaintained.com/badge/open/shibdib/API-Registration-Mod-Revisited.svg)](http://isitmaintained.com/project/shibdib/API-Registration-Mod-Revisited "Percentage of issues still open")


Cyerus brought us this mod and it's up to us to keep it running smoothly. Pull requests highly encouraged.


Requirements
-----------
```
- Apache2 Server
- Database of some sort (Preferably MYSQL)
- PHP Installed
```

Install
-----------
```
1. Install a clean version of phpBB 3.0.14 and AUTOMOD

2. Download the latest FULL release as a .zip and install using AUTOMOD

3. Clear forum cache

4. Go to *url.com*/install and select install

5. Once installed, delete the install folder from your forum

6. Use AUTOMOD to install the mod into your theme of choice

7. Be sure to setup a cronjob to run the eveapi_cron.php file in your forum root directory. Recommended not to do it more than once every three hours or risk false positives because of API timeouts.
```

Database Update
-----------
```
The latest database item update is included in the db folder and must be manually added to your mysql install.

This is most easily done using phpmyadmin but can be done from the command line as well with the following command

mysql -u username -p database_name < file.sql   (with database_name being the name of your forum database, and file.sql being the full path to the sql file in the db folder.)
```

Full Update
-----------
```
1. Uninstall EVE API x.x.x from the AutoMOD section of the ACP.

2. Clear forum cache

3. Upload and install EVE API x.x.x to the AutoMOD section of the ACP.

4. Clear forum cache again

5. Go to forum.com/install and select update

6. Once installed, delete the install folder from your forum

7. Use AutoMOD to make the required changes to your custom template (if required)

8. Cycle through each of the EVE API setting pages and save them

9. Cycle through each of the forum group setting pages and save them

10. Clear forum cache one last time, and we should be done.
```

