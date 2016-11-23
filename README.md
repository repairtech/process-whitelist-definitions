Hey techs!

This is the whitelist for RepairTech's new process killer tool. The tool is meant to kill unnecessary processes before scanning for malware. It can whitelist processes based on a bunch of different properties. Here's where we need your help! We have open-sourced the whitelist on github, and would like your suggestions for more whitelisted items before we release the tool.

This whitelist includes 4 different properties it can sort by. I'll explain how to find each one in a normal application:

 - User - The user running the process. Just open Task Manager and see which User owns that process.
 - Product Name - Right click on an executable, go to Properties -> Details, and you'll see "Product name".
 - Signature - If the executable is digitally signed, we can filter by any of the properties of that signature.
 - Process Name - The name of the process that you see in Task Manager.
 
A couple things to note:

 - Everything is case-insensitive
 - Each line is a separate list
 - We will match parts of words. So far example if the process name is "TeamViewerQS.exe" and we whitelist "TeamViewer" it will be a match because "TeamViewer" is a part of "TeamViewerQS.exe"

If you have suggestions for additions to the whitelist, you can either send us an email at support@repairtechsolutions.com, or you can open an "Issue" on Github. 
