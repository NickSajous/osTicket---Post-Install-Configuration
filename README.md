<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure roles, departments, Teams, etc 
- Acknowlegde Agent Panel vs Admin Panel
- Prepare osTicket to recieve mock tickets

<h2>Configuration Steps</h2>

<p>
*IMPORTANT* At the top right of the screen, you'll see either "Agent Panel" or "Admin Panel" (as shown below). We will be switching back and forth between the two of these panels in this tutorial.
</p>
<p>

  ![Screenshot 2025-04-28 162234](https://github.com/user-attachments/assets/e3decbd7-bfd7-4a22-94e5-c0923d7e6814) ![Screenshot 2025-04-28 162317](https://github.com/user-attachments/assets/7913bea7-fa9b-4455-a611-f9a1c360a7e3)


</p>
<br />

<p>
1. In the Admin Panel, click on "Agents", then select "Roles" and click "Add New Role". Type in "Supreme Admin", then go to the "Permissions" tab and check all the check boxes under all the sub-categories then click on "Add Role". You should see the Supreme Admin role you just created in the drop down list. (show below)
</p>
<p>

  ![Screenshot 2025-04-28 163026](https://github.com/user-attachments/assets/11af6eb7-4904-4aa3-96e7-762e359d95d1) ![Screenshot 2025-04-28 163046](https://github.com/user-attachments/assets/d8c697a3-0e1c-4c03-87b8-e52d3f47c8f4)  ![Screenshot 2025-04-28 163137](https://github.com/user-attachments/assets/5c1aad92-0848-4d29-8545-9724c38bde3e) ![Screenshot 2025-04-28 163547](https://github.com/user-attachments/assets/97216dde-176a-42b7-880b-1cffdf2cee14)





</p>
<br />

<p>
2. From the same screen, click on "Departments", then add a new department. When you do, leave everything as is except for the name. Type "SysAdmins". At the bottom of the screen, click "Create Dept". You should see the department you created in the list of names.
</p>
<p>

  ![image](https://github.com/user-attachments/assets/b37dd806-5213-44aa-8490-ecbc22fefd72) ![image](https://github.com/user-attachments/assets/331fe0c2-5f69-4410-9337-3cf7f8bbed2a) ![image](https://github.com/user-attachments/assets/874993ce-b4bc-4bdb-b740-8af6be9e838c)



</p>
<br />




</p>
<br />

<p>
3. Click on "Teams" under the "Agents" category. Click "Add New Team" and name it "Online Banking". You can leave everything else as is and click "Create Team" at the bottom of the screen.  
</p>
<p>

  ![image](https://github.com/user-attachments/assets/1a7030b4-ecf4-487d-bf22-a06e1bf00a18) ![image](https://github.com/user-attachments/assets/7b8e1762-756b-41dd-b542-43f5f31ab32d)


</p>
<br />




</p>
<br />

<p>
4. *IMPORTANT* Go to "Settings", then "Users". Make sure that the "Registration Required" checkbox is unchecked.
</p>
<p>

  ![image](https://github.com/user-attachments/assets/9593e494-3c52-4255-9c7f-be24c9a7ca73)

</p>
<br />




</p>
<br />

<p>
5. Go back to "Agents", then click "Add New". For the first and last name, you can type in "Jane Doe". For the email address, you can put any fake email address. For this instance, we're going to put Jane@lognpacific.com. For the username type in "jane". Click on "Set Password" and uncheck the checkbox. Set the password to "Password1", then click "Update". Under the "Access" section, "Select SysAdmins" from the drop down menu, then select "Supreme Admin" in the other drop down menu. Under the "Teams" section, select "Online Banking" from the drop down menu. Click Create.
</p>
<p>

  ![image](https://github.com/user-attachments/assets/0e9cd41a-775d-446b-9fe7-cdcf12cd5b29) ![image](https://github.com/user-attachments/assets/3feb86fa-05d8-40c3-b0d6-3c20062f789c) 
![image](https://github.com/user-attachments/assets/58f70f0c-a874-44e6-9aed-0535622de791) ![image](https://github.com/user-attachments/assets/7fcd71fb-c9f1-4cb8-926d-391cbf5b719a) 



</p>
<br />




</p>
<br />

<p>
6. When finished creating Jane, Add another agent named John. Type in "John Doe" for the first and last name and John@lognpacific.com for the email. Click on "Set Password" and uncheck the checkbox. Set the password to "Password1", then click "Update". Under the "Access" tab, select "Support" from the drop down menu. When finished, click create. 
</p>
<p>

  ![Screenshot 2025-04-28 185639](https://github.com/user-attachments/assets/3da2c85f-8210-4ea0-a413-eab0776d05d7) ![Screenshot 2025-04-28 185720](https://github.com/user-attachments/assets/7f244ff3-a3d3-4903-98be-f7b98acc524b)


</p>
<br />



<p>
7. *SWITCH TO THE AGENT PANEL* Under the "Users" tab, click "Add Users". Type in "karen@lognpacific.com" for the email, and type in "Karen" for the name. Click "Add User" when finished. 
</p>
<p>

![image](https://github.com/user-attachments/assets/aa9aaa2c-4aa2-4aa9-bb3b-654c0c75bdc5) ![image](https://github.com/user-attachments/assets/95f48812-879c-43b0-8535-e7daeb2da3c5)




</p>
<br />





<p>
8. *GO BACK TO THE ADMIN PANEL* Under the "Manage" tab, click "SLA", then "Add New SLA Plan". Type in "Sev-A" for the name, set the grace period to "1", and set the schedule to "24/7". This is the most urgent sev (severity). Do this two more times for "Sev-B" and "Sev-C". for Sev-B, type "4" for the grace period, and select "24/7" from the "Schedule" drop down menu. For Sev-C, type "8" for the grace period, and select "Monday - Friday 8am - 5pm with U.S. Holidays" from the "Schedule" drop down menu.
</p>
<p>

![image](https://github.com/user-attachments/assets/c0a5664c-bfa0-40dd-ac97-b62465e81223) ![image](https://github.com/user-attachments/assets/63057ac5-0307-4039-9e90-a17e3b8de081) ![Screenshot 2025-04-28 194407](https://github.com/user-attachments/assets/ca9a94f5-8d25-410f-b024-3e0b6a9af240) ![Screenshot 2025-04-28 194431](https://github.com/user-attachments/assets/42c4e22b-25f3-4892-8078-a69d882963a3)





</p>
<br />





<p>
9. In the "Manage" tab, click "Help Topics". Create 5 help topics named "Business Critical Outage", "Personal Computer Issues", "Equipment Request", "Password Reset",and "Other". In the "Parent Topic" drop down menu, select "General Inquiry" for "Equipment Request" and "Other". Select "Report a Problem" for the rest of the 3 categories.



</p>
<p>

![Screenshot 2025-04-28 195816](https://github.com/user-attachments/assets/9387a42b-5c32-4a2a-b240-f501457adef8)
 


</p>
<br />
