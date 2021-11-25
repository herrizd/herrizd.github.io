---
layout:     post
title:      Use Power Automate – save emails to OneDrive
subtitle:   
date:       2021-11-19
author:     Herriz
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - Power Automate
    - Office skills
---

##  



| **Last Update:** | 20-Nov-21                                                    |
| ---------------- | ------------------------------------------------------------ |
| **Title:**       | Use Power Automate – save emails to OneDrive                 |
| **Purpose:**     | To create a flow automatically to save all the emails received in a email account including the attachments |
| **Help video:**  | https://web.microsoftstream.com/video/8665a635-c160-4762-9cd2-fc64dc61d7d6 |



Instructions


1. Access the Microsoft Power Automate portal: https://flow.microsoft.com/ and sign in with your account.

2. Create a flow with Automated trigger **When a new email arrives** ,If you only want specific newsletters to be copied, click **Show advanced options** to narrow down trigger conditions. Then click  **New Step** to  create an **get email** trigger, Click on the **Message Id**，this will help you get more information from new email. Once you’re done, click **New Ste**p and add an action **Export email**. Click on the **Message Id**. Then, in the popup on the right, find dynamic content called **Message Id**. Add an action **Create file**. This is where you will specify the location and properties of your newsletter copy   
   
5. The final flow structure should look like this:

    ![image-20211124152627466](C:\Users\k56678\AppData\Roaming\Typora\typora-user-images\image-20211124152627466.png)





