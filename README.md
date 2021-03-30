Get browsers history in Windows systems - Opera, Chrome, Yandex, Brave, Firefox.
To get access to the history files one preventionally needs to have admin access to remote machine (Active Directory admin rights and so on).
Also one needs sqlite3.exe as a pre-requisite. One may execute the next commands on local machine to get sqlite3.exe:
1. powershell -c "Invoke-WebRequest -Uri 'https://sqlite.org/2021/sqlite-tools-win32-x86-3350300.zip' -OutFile 'c:\sqlite3.zip'"
2. powershell -c "Expand-Archive -Force C:\sqlite3.zip C:\sqlite3"
3. del /Q C:\sqlite3.zip
4. mv C:\sqlite3\sqlite-tools-win32-x86-3350300\sqlite3.exe \path_you_like
5. rmdir /Q /S C:\sqlite3

Tested on Windows 10 and last date browsers.
