# OutlookProfileTool
Reset Outlook Profile tool after migration

This application is available for partner testing. Pleae reach out with any questions.

This activity requires PowerShell capability by the partner to configure the tool.

Revision (2021/03/20):
1.	$Script:MigrateMsgOutlookOpened and $Script:MigrateMsg were swapped for messaging. Fixed the wording on those (lines 11 and 13)
2.	Changed .\ with $PSScriptRoot on lines 22 and 371. Using .\ can be problematic if the script is ran without the working directory set properly.
It’s best to use $PSScriptRoot as this variable gets replaced with the path the script is being ran from.
3.	In the config file you had C:\Program File\XXX. This worked because Program File was missing the s.
The logging path to C:\Program Files\foldername it will fail as you need local admin rights to write to C:\Program Files\x.
C:\OutlookScriptLogs to prevent this error just in case.
-Marc Arsenault

MS dll Search - This code is to assist organizations that have multiple .NET deployments. It is prepared to look for the specific library files. This will replace the the hardcoded path for the MS .NET libraries. This code has not been tested by SSC. If you have any questions please reach out for assistance. - Mike Money
