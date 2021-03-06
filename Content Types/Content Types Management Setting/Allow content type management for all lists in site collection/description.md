A short Powershell script to allow management of content types for all SharePoint Online lists and libraries across all sites in a site collection

 

It is an equivalent of List>>List Settings>>Advanced>>Content types in Graphic User Interface (see screenshot)

 



 

 

Applies to lists and libraries.

 

 

It requires installed  SharePoint Online SDK

You have to enter the list information before running the script:

 

```PowerShell
 
# Paths to SDK. Please verify location on your computer. 
Add-Type -Path "c:\Program Files\Common Files\microsoft shared\Web Server Extensions\15\ISAPI\Microsoft.SharePoint.Client.dll"  
Add-Type -Path "c:\Program Files\Common Files\microsoft shared\Web Server Extensions\15\ISAPI\Microsoft.SharePoint.Client.Runtime.dll"  
 
# Insert the credentials and the name of the site and the desired setting: $true for the content types management to be allowed or $false to disable it 
$Username="trial@trialtrial123.onmicrosoft.com" 
$AdminPassword="Pass" 
$Url="https://trialtrial123.sharepoint.com/sites/teamsitewithlists" 
$ContentTypesEnabled=$true 
``` 
 

 

 

Please share your thoughts in the Q&A section!

 

Wiki article with detailed code description:
 

[SharePoint Online: Turn on support for multiple content types in a list or library using Powershell](http://social.technet.microsoft.com/wiki/contents/articles/30038.sharepoint-online-turn-on-support-for-multiple-content-types-in-a-list-or-library-using-powershell.aspx)

 

Related scripts
Set-SPOList properties (module)

Disable or enable attachments to list items using Powershell

Change search setting for all lists in a site using CSOM and Powershell

Allow content type management for all lists in a site using Powershell

Set content type management setting for SharePoint Online list using Powershell


<br/><br/>
<b>Enjoy and please share feedback!</b>
