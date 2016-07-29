# Install-Curl
Set of scripts and programs to install cURL 7.50.0 (as of 2016-07-29). Substitute for http://www.confusedbycode.com/curl/ and https://chocolatey.org/packages/curl which are both out of date.

<#
.Synopsis
   Automatically install cURL in Windows
.DESCRIPTION
   A script that can either copy a local copy of cURL to either a specified directory or default install directory or download from a specified or pre-specified location. 
.EXAMPLE
   Install-Curl.ps1
.EXAMPLE
   Install-Curl.ps1 -installDirectory "C:\Temp" -Force32BitInstall -ForceDownload -32BitDownloadLocation "https://bintray.com/artifact/download/vszakats/generic/curl-7.50.0-win64-mingw.7z"
.INPUTS
   $installDirectory
   $Force32BitInstall
   $ForceDownload
   $32BitDownloadLocation
   $64BitDownloadLocation
.NOTES
   Running the script as is will copy curl.exe and ca-bundle.crt to their respective architecture and default install location and if it can't find those files, will download it from winamppugins.co.uk   
#>