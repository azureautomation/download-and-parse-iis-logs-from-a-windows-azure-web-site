Download and Parse IIS logs from a Windows Azure Web Site
=========================================================

            

[Windows Azure Scripting Center](http://www.windowsazure.com/en-us/documentation/scripts) |
[Get Started with Windows Azure PowerShell](http://go.microsoft.com/fwlink/?linkid=320929&clcid=0x409) |
[Windows Azure Web Scripts](http://www.windowsazure.com/en-us/documentation/scripts/index/?solution=web&service=all)

Description

Downloads IIS logs from an Azure Website and searches the log for any HTTP 400 and above status codes.


If Http logging is not enabled on the website, then it will enable logging if the EnableHttpLogging switch is specified.


The downloaded logs are unzipped and then fed into LogParser (if installed), querying for any HTTP status codes 400 and above. The output of the LogParser query is output to the console.


**Note:** This script requires an Azure Storage Account to run. The storage account can be specified by setting the subscription configuration. For example,


Set-AzureSubscription -SubscriptionName 'MySubscription' -CurrentStorageAccount 'MyStorageAccount'

Example
 
Scenario
You want to quickly check the IIS logs for an Azure Website to find HTTP errors.
Requirements

  *  PowerShell Version 3.0 
  *  Windows Azure PowerShell 0.6.18 
See Also

  *  [Set-AzureSubscription](http://msdn.microsoft.com/en-us/library/windowsazure/dn408531.aspx)

  *  [Windows Azure Web Scripts](http://www.windowsazure.com/en-us/documentation/scripts/index/?solution=web&service=all)

Script Content

The content of the script is reproduced below

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
