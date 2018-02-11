## Use HTAccess to Password Protect Your Web Pages/Folder/File

**Step1**  Open the folder which is not public or accessible using webaddress.
**Step2**  Create a file '.htpasswd' using commnad 
           1.  vi .htaccess
           2.  Add following lines to your file and save the file.
           ```python
s = "Python syntax highlighting"
print s
```
 
```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```
           ```
           username
           password
           ```
      
**Step3** Open the webpage folder or file to which you want to add privacy settings.
**Step4** Create a file '.htaccess' using commnad 
           * vi .htaccess
           
**Step5** Add Following lines to the '.htaccess' file.
            ```
              AuthUserFile /path/to/htpasswd/file/.htpasswd
              AuthGroupFile /dev/null
              AuthName "Name of Area"
              AuthType Basic
              require valid-user
              ```
          1. In the above line1 change path from '/path/to/htpasswd/file/.htpasswd' to the path of the folder containing '.htpasswd' file.
          2. In the above line3 change Auth Name from 'Name of Area' to the name you want the dialog box to show.(Not necessary).
          3. Save the file
      
**Step6** Open your webpage in the browser, it will prompt for login, enter your username and passwd. 

**Done **
          


   


