---
layout:     post
title:      Use Power Automate – save emails to OneDrive
subtitle:   Automatically 
date:       2021-11-19
author:     Herriz
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - Power Automate
    - Office365 skills
---

[TOC]



<h2 id="1">EN</h2>
<h2 id="1">CH</h2>

##  Instructions



| **Last Update:** | 20-Nov-21                                                    |
| ---------------- | ------------------------------------------------------------ |
| **Title:**       | Use Power Automate – save emails to OneDrive                 |
| **Purpose:**     | To create a flow automatically to save all the emails received in a email account including the attachments |






1. Access the Microsoft Power Automate portal: https://flow.microsoft.com/ and sign in with your account.

2. Create a flow with Automated trigger **When a new email arrives** ,If you only want specific newsletters to be copied, click **Show advanced options** to narrow down trigger conditions. Once you’re done, click **New Step** and add an action **Office 365 Outlook – Export email**.
    Click on the **Message Id**. Then, in the popup on the right, find dynamic content called **Message Id**.          ![image-20211124132542480](C:\Users\k56678\AppData\Roaming\Typora\typora-user-images\image-20211124132542480.png)

3. Add an action **Export email**

4. Add an action **Create file**. This is where you will specify the location and properties of your newsletter copy:

    **Site Address**: specify your target site URL. Normally, you should find it in the drop-down list.
    **Folder Path**: add the name of the destination library.
    **File Name**: here you can get creative and mix static text with multiple values from the dynamic content drop-down. Or you could simply add **Subject**. Now, if you want the file to be readable by your browser, add *.eml* or *.mht* suffix at the end and see which format works best for you.
    **File Content**: add **Body** from dynamic content drop-down.
    Save and test your flow. If you encounter errors, double-check file paths: the problem is most likely there.

5. The final flow structure should look like this:

    ![image-20211124152627466](C:\Users\k56678\AppData\Roaming\Typora\typora-user-images\image-20211124152627466.png)

[点击跳转](#Instructions)



