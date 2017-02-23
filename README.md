# Install-Curl
Set of scripts and programs to install cURL 7.53.0 (as of 2017-02-23) to Windows. Substitute for http://www.confusedbycode.com/curl/ and https://chocolatey.org/packages/curl which are both out 
of date.


##Description
Takes either a local copy of curl and ca-bundle.crt or one downloaded from the internet, installs it to Program Files, and adds the path to the System PATH environment variable. 
Supports 32-bit and 64-bit versions of cURL. You can specify the install directory, download location, and can force a 32-bit install. If downloaded from the internet, currently 
only supports 7zip format.

##Example
Install-Curl.ps1 

##Example
Install-Curl.ps1 -installDirectory "C:\Temp" -Force32BitInstall -ForceDownload -32BitDownloadLocation "https://bintray.com/artifact/download/vszakats/generic/curl-7.50.0-win64-mingw.7z"

##Inputs
$installDirectory  
$Force32BitInstall  
$ForceDownload  
$32BitDownloadLocation  
$64BitDownloadLocation  

##Notes
Running the script as is will copy curl.exe and ca-bundle.crt to their respective architecture and default install location and if it can't find those files, will download it from winamppugins.co.uk   