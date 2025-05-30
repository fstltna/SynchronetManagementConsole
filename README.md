# Synchronet BBS Management Console (1.26.2)
Allows you to manage your Synchronet BBS server with a text based UI - 
Official support sites: [Official Github Repo](https://github.com/fstltna/SynchronetManagementConsole) - [Official Forum](https://synchronetbbs.org/index.php/forum/synchronet-management-console)
![Synchronet Logo](https://SynchronetBBS.org/SynchronetLogo.png)

[Join our Discord Server](https://discord.gg/Q5KBBKY)

---

Run smc, then use the "edit settings" option if your Synchronet BBS server is not in "/sbbs".

You will need to run ./installdeps

You also need to have my Synchronet BBS Startup Script and Synchronet BBS Backup Script installed.

I then suggest you add this directory (SynchronetManagementConsole) into your path, so that you can just run "git pull" to upgrade to the latest version as updates come out. Put this at the top of your .bashrc file:

>export PATH=/home/bbsowner/SynchronetManagementConsole:$PATH


***

1. "8 - Back Up BBS" - As it says this backs up your BBS folder tree.
2. "9 - Set File Perms" - If you have recompiled anything you should run this option to reset the permissions of the BBS tree to allow sbbs to open low ports.
3. "10 - Call Outs Menu" - Links to force manual call-outs to other networks
4. "11 - Edit Settings" - Edit the settings used in SMC itself. Should not need changes but it is here just in case. You can edit the "debugmode" option to "on" to display each command that will be run before executing them.
5. "12 - Reset BBS Processess" - Resets just the BBS process so it can be automaticly restarted.
6. "13 - Posting Tools" - Brings up the posting tools menu.
7. "14 - Log Files" - Brings up the log file tools menu.
8. "15 - Log Files" - Brings up the log file tools menu.
9. "16 - Update Tools" - lets you update to latest versions of these tools

Refer to this menu for what follows:

![](https://SynchronetBBS.org/SMC_Images/SMC_PostingMenu.png) 


1. "1 - Edit Announce.txt" - This is the text that will be used by the #4 "Run BBS Announce" option. This posts about your BBS to the selected groups as set up in the #6 "Edit BBS IDs" option.
2. "2 - Edit FilePost.txt" - This is the text that is shown before the list of files as sent in the #5 "Run FileAnnounce" option.
3. "3 - Edit FilePostBottom" - This is the text that appears after the files as sent in the #5 "Run FileAnnounce" option.
6. "6 - Edit BBS IDs" - This is the settings tha the #12 "Run BBS Announce" option uses to post your messages.![](https://SynchronetBBS.org/SMC_Images/SMC_BBS_IDS.png) 
7. "7 - Edit File IDs" - This is the settings tha the #5 "Run File Announce" option uses to post your messages.![](https://SynchronetBBS.org/SMC_Images/SMC_FILE_ID.png) 
