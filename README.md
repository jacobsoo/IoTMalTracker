# IoTMalTracker
This repo will contain the SQLite file(s) containing the IoT malware that my tracker found.

I will not be publishing the codes to my IoT Malware Tracker for now.
The backup to the SQLite files are found here.
https://mega.nz/folder/NkFSlBCa#8zWYvIoW8hSfda0qN8j3KA



This is the structure of the SQLite file. 

The `FILE` column contains the actual IoT malware that my tracker grabbed.
```sql
CREATE TABLE "Malwares" (
                            `ID` INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT, 
                            `LOCATION` TEXT NOT NULL, 
                            `TYPE` TEXT, 
                            `MD5` TEXT NOT NULL, 
                            `SHA1` TEXT NOT NULL, 
                            `SHA256` TEXT NOT NULL, 
                            `FILE` BLOB NOT NULL,
                            `DATE` DATE, 
                            `COMMENTS` TEXT, 
                            `TAGS` TEXT );
```
