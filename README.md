# Change Windows 10 Edition Eval

Step1: Copy to C:\Windows\System32\spp\tokens\skus
#
Step2: Using cmd as an Administrator

cscript.exe %windir%\system32\slmgr.vbs /rilc

cscript.exe %windir%\system32\slmgr.vbs /upk >nul 2>&1

cscript.exe %windir%\system32\slmgr.vbs /ckms >nul 2>&1

cscript.exe %windir%\system32\slmgr.vbs /cpky >nul 2>&1

cscript.exe %windir%\system32\slmgr.vbs /ipk NPPR9-FWDCX-D2C8J-H872K-2YT43

sc config LicenseManager start= auto & net start LicenseManager

sc config wuauserv start= auto & net start wuauserv

clipup -v -o -altto c:\

echo
#
Step3: Using an Product key to activate Windows 10 Enterprise
