# Intro to Keepass for Shared Passwords

Keepass is an free open-source multi-platform password manager



> You can store all your passwords in one database, which is locked with a master key. So you only have to remember one single master key to unlock the whole database. Database files are encrypted using the best and most secure encryption algorithms currently known AES-256.

To access the RCODI password database you will need the following:

1. **A keepass client** (the official keepass application, keeweb, or any of the many other open-source apps that are compatible with the keepass database)
    - https://keeweb.info/ 
    - https://keepass.info/help/v2/setup.html
    - https://keepass.info/plugins.html
    
2. **A copy of the RCODi Keepass database file (.kdbx)** 
    - You can download the current up-to-date dbx at:
             `***/ RCODI Dropbox /Admin Docs / passwords***` 
            
    - You should download or copy the kdbx file to a new location on your computer that is not being synced to Dropbox.
    - If you add a new password or make changes to an existing record then you should then upload the new version to dropbox **AND overwrite the existing file.** 
    - Do NOT make copies or versions of the password database. This will make it impossible to know which version has the correct password for any of the accounts and will make everyone sad.
    - Dropbox continuously watches files on your computer for chages and uploads file fragments every time there is a change. Working with the kdbx file directly on the dropbox folder will not cause an errors but the more people that use the shared the more likely that the integrity of the file will be corrupted if two people save new data at the same time. Early  Keepass database files had a reputation for becoming corrupted and unopenable especially when they were being used between windows and mac environments. We will always be able to revert back to a previous vesion on Dropbox but you should take steps to avoid unecessary extra work and trouble.
----------
https://www.dropbox.com/s/msb79xel2r0ny7i/rcodi-keepass.kdbx?dl=0
https://www.dropbox.com/s/lzby8sy1hzciaiu/rcodi-keepass.key?dl=0

3. **A copy  of the database encryption key file**

Also download the key file when you get the .kdbx file. Put the key file somewhere in your user directory that is not /Downloads folder or dropped on your desktop. You should not share this file or send it directly to yourself or anyone else over the internet.  Once you pick an appropriate place you will not have to update or touch this file again. 

4. **Know the database password.** 

Keepass uses a two part encryption system that uses a password along with the key file together to produce the overall key that can unlock the database. 

**STEPS AFTER COMPLETING 1-4:**

- Open keepass/keeweb 
- Select ‘Open’ from the screen 
- Select the ‘rcodi.kdbx’ file in the file chooser
- Below the password input box there is a button in the shape of a key, click this and select the ’rcodi.key’ file this time.
- Enter the correct password and you can start using keepass

Theres are lots of useful features you can take advantage of including

    - Using keepass to create random passwords for you
    - Keepass lets you store images and files in the database as well for things like QR codes
    - Add icons, labels, and color code groups for your passwords
    - Add text and markdown formatted text in the notes for more useful entries
    - Connect your keepass/keeweb with cloud storage and automate backups using dropbox or google drive’s App API (not the same as putting a file in sync storage)
    - Change the theme
    - Run in the app in background so you dont have to find it every time you need  password

Suggestions:

    - If the RCODI keepass database is the only thing you are using keepass for you will most likely have a hard time remembering the password when you eventually need to use it. 
    - What you SHOULD NOT do is revert to writing the keepass password on a sticky note in your desktop or save a screenshot of it in the same folder so you can find. This type of practice makes all of the effort to use a password manager effectively useless.  
    - An easy way to set up a system so you can always be able to find the password when needed it to create a new kdbx for personal use, you can use a personal password for this file that you will remember and inside you should keep the RCODI kdbx password along with other notes that you might need. 
    - If you do this and still feel like you might forget this other password, you should use the Google Chrome password manger as a backup backup. If you use the web interface for keeweb you can save the credentials in Chrome. or just go to chrome://settings in the url bar then click ‘passwords’ and add it directly
    
----------


![1](https://paper-attachments.dropbox.com/s_96950934E8BFEA3E0FAFAD81101EFCA8CAD936B917733F3F98B261B756E50701_1586560872339_Screenshot+from+2020-04-10+17-24-48.png)

![2](https://paper-attachments.dropbox.com/s_96950934E8BFEA3E0FAFAD81101EFCA8CAD936B917733F3F98B261B756E50701_1586560872344_Screenshot+from+2020-04-10+17-28-15.png)

![](https://paper-attachments.dropbox.com/s_96950934E8BFEA3E0FAFAD81101EFCA8CAD936B917733F3F98B261B756E50701_1586560872357_Screenshot+from+2020-04-10+17-29-11.png)

![](https://paper-attachments.dropbox.com/s_96950934E8BFEA3E0FAFAD81101EFCA8CAD936B917733F3F98B261B756E50701_1586560872363_Screenshot+from+2020-04-10+17-29-34.png)
![set a password expiration date](https://paper-attachments.dropbox.com/s_96950934E8BFEA3E0FAFAD81101EFCA8CAD936B917733F3F98B261B756E50701_1586560872369_Screenshot+from+2020-04-10+17-29-44.png)
![add a new field to a record](https://paper-attachments.dropbox.com/s_96950934E8BFEA3E0FAFAD81101EFCA8CAD936B917733F3F98B261B756E50701_1586560872375_Screenshot+from+2020-04-10+17-29-55.png)

![](https://paper-attachments.dropbox.com/s_96950934E8BFEA3E0FAFAD81101EFCA8CAD936B917733F3F98B261B756E50701_1586560872381_Screenshot+from+2020-04-10+17-30-55.png)


