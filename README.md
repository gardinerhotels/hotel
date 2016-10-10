# Mastering ServiceNow - Second Edition

This GitHub repository contains the Hotel application built out in the Mastering ServiceNow book.  To get started quickly, please fork this Hotel repository at GitHub.  Use the **Fork** button just up there to the right.  You will need a GitHub account to carry this out, but don't worry, its free.

You will then be redirected to your fresh copy. Take the URL from your browser (it will be `github.com/<username>/hotel`) and follow these instructions.

## Importing the application

Linking your application to your new repo is easy! Just follow these steps in your ServiceNow instance.  Note it must be running the **Helsinki** version of ServiceNow.

1.  Navigate to **System Applications** > **Studio**, and click on **Go** next to **Open studio**.
2.  In the window that appears, click **Import From Source Control**
3.  Fill out the URL, User name and Password with the URL you copied just now, and your Github credentials
4.  Click **Import** and let the magic happen!
5.  Once it is done, click **Select Application**, then click **Hotel** in the list. You are done! You now have the 

## Jumping to another branch

The Source Control feature of Studio allows you to make _checkpoints_, letting you jump to a particular version very easily. I have created a branch for each chapter. This means that if you wish to start with Chapter 11 (and have fun with Service Portal), you can check out Chapter 10 and get straight to it. So while every chapter builds on the previous one, you can type in the cheat code and jump to where you want.

Follow these steps to do so:

1.  Open up Studio: **System Applications** > **Studio**, and click on **Go** next to **Open studio**. Select **Hotel**.
2.  From the **Source Control menu**, click **Switch Branch**.
3.  If you have done configuration, you will need to decide if you want to get rid of it, or _stash_ it. Select the appropriate option.
4.  In the dropdown, select the branch you want. If you want to import all of the configuration from Chapter 7 _and all previous chapters_, select **07-Integrations** and click **Switch Branch**.
5.  Wait while the your application is aligned to that in the repo, and once done, click **Close Dialog**
6.  To manage your stashes, you can, erm, click **Manage Stashes** in the **Source Control** menu

Some supporting data have been added to each branch. This includes some example Room and Maintenance records, as well as some test users.  The `admin` user contains the necessary roles to work with application, so has been included from Chapter 8 onwards. The Active, Locked Out and Password fields will not be altered however.  If you have difficulty accessing the Hotel application, use the admin user to access it.

## Disabling Scoped Administration
Scoped Administration only allows users with the right roles to access the application.  This include System Administrators.  If you wish to disable this (enabled from Chapter 8 onwards), import [this XML file](https://www.gardiner-hotels.com/sets/sys_app_hotel.xml) to update the Scoped administration field appropriately.
