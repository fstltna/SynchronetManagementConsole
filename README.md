# Synchronet BBS Management Console (1.4.0)
Allows you to manage your Synchronet BBS server with a text based GUI - 
Official support sites: [Official Github Repo](https://github.com/fstltna/SynchronetManagementConsole) - [Official Forum](https://synchronetbbs.org/index.php/forum/synchronet-management-console)
![Synchronet Logo](https://SynchronetBBS.org/SynchronetLogo.png)

[![Visit our IRC channel](https://kiwiirc.com/buttons/irc.synchro.net/SynchronetFans.png)](https://kiwiirc.com/client/irc.synchro.net/?nick=guest|?#SynchronetFans)

---

Run the smc console once, then use the "edit settings" option if your Synchronet BBS server is not in "/sbbs".

You will need to run cpan and install these modules:

- UI::Dialog
- Term::ReadKey
- Term::ANSIScreen
- Proc::ProcessTable

You also need to have my Synchronet BBS Startup Script and Synchronet BBS Backup Script installed.

I then suggest you add this directory (SynchronetManagementConsole) into your path, so that you can just run "git pull" to upgrade to the latest version as updates come out. Put this at the top of your .bashrc file:

>export PATH=/root/SynchronetManagementConsole:$PATH


***

1. "8 - Back Up BBS" - As it says this backs up your BBS folder tree.
2. "9 - Set BBS Owner" - If you have made any changes in scfg or through the shell you should run this option to reset the owner of the BBS tree to the BBS owner and not "root" or other users.
3. "10 - Call DOVENET" - Tell the BBS to check Dovenet for new data right away.
4. "11 - Edit Settings" - Edit the settings used in SMC itself. Should not need changes but it is here just in case. If you make any changes here you need to exit SMC and relaunch it again.
5. "12 - Call NEWSLINK" - Tell the BBS to check Newslink/USENET for new data right away.
6. "13 - Reset BBS Processess" - Resets just the BBS process so it can be automaticly restarted.
7. "14 - Posting Tools" - Brings up the posting tools menu.

Refer to this menu for what follows:

![](https://SynchronetBBS.org/SMC_Images/SMC_PostingMenu.png) 


1. "1 - Edit Announce.txt" - This is the text that will be used by the #4 "Run BBS Announce" option. This posts about your BBS to the selected groups as set up in the #6 "Edit BBS IDs" option.
2. "2 - Edit FilePost.txt" - This is the text that is shown before the list of files as sent in the #5 "Run FileAnnounce" option.
3. "3 - Edit FilePostBottom" - This is the text that appears after the files as sent in the #5 "Run FileAnnounce" option.
6. "6 - Edit BBS IDs" - This is the settings tha the #12 "Run BBS Announce" option uses to post your messages.![](https://SynchronetBBS.org/SMC_Images/SMC_BBS_IDS.png) 
7. "7 - Edit File IDs" - This is the settings tha the #5 "Run File Announce" option uses to post your messages.![](https://SynchronetBBS.org/SMC_Images/SMC_FILE_ID.png) 
