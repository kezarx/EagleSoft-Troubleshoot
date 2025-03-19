# EagleSoft-Troubleshoot

There is an error in Eaglesoft when you try to login 

Error Code:  [Microsoft][ODBC Driver Manager] Data source name not found and no default driver specified

First step will be to open up a Adminsitrator CMD and go to 

open CMD -> cd C:\Eaglesoft\Shared Files -> OcxReg.exe -UNREG | then run OcxReg.exe -REG

Also best to open taskmanager on the PC to make sure OCXREG.exe -UNREG has fully run before running the OCXREG.exe -REG 

If this does not fix the issue, you will need to rename a file. 

rename Eaglesoft.Client.Configuration.data to Eaglesoft.Client.Configuration.data_old 

(note: Please close out of any running instance of Eaglesoft before performing these steps and the steps above (OCXREG.exe steps)) 

reopen Eaglesoft and it should create a new Eaglesoft.Client.Configuration.data 

now test the login. 
