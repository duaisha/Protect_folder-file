## Use HTAccess to add privacy settings to your Web Pages

* **Step1**  Open the folder which is not public or accessible using webaddress.
* **Step2**  Create a file '.htpasswd' using commnad 
           1.  vi .htaccess
           2.  Add following lines to your file and save the file.

```
username
password
```

* **Step3** Open the webpage folder or file to which you want to add privacy settings and is in public_html.
* **Step4** Create a file '.htaccess' using commnad 
           * vi .htaccess
           
* **Step5** Add Following lines to the '.htaccess' file.
```
AuthUserFile /path/to/htpasswd/file/.htpasswd
AuthGroupFile /dev/null
AuthName "Name of Area"
AuthType Basic
require valid-user
```
**<span style="color:blue">Do the following changes to above code</span>**

1. Change the path in line1  from "/path/to/htpasswd/file/.htpasswd" to the path of the folder containing .htpasswd file.
2. Change the auth name in line3 from "Name of Area" to the name you want the dialog box to show.(Not necessary).
3. Save the file
      
* **Step6** Open your webpage in the browser, it will prompt for login, enter your username and passwd. 

* Done
          



