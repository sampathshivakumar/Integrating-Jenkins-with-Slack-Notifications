## Integrating Jenkins with Slack Notifications.
![slack](https://user-images.githubusercontent.com/119833411/241564634-bc981dab-898e-49d1-882d-f3290551c355.jpg)
### Prerequisites:
* **A Jenkins Server which is up and running.**
* **A Slack Account.** 

**You can see Jenkins Step by Step Installation here.** https://gist.github.com/sampathshivakumar/54449ea95540ad0fd0f0cf44beb54ff9

**You can sign up for a Slack account here.** https://slack.com/intl/en-in/

### Lets signup for a account 1st.
![1](https://user-images.githubusercontent.com/119833411/241567268-c8e4b31a-6c9f-4ab1-ac24-22890f2eb7ae.jpg)

**Signup with gmail and click Confirm.**

![2](https://user-images.githubusercontent.com/119833411/241567620-21301e51-7ee0-4fdd-829a-a9919b7663a6.jpg)

**Now Create a Workspace.**

![3](https://user-images.githubusercontent.com/119833411/241567888-237db977-c9b3-479a-8552-59d34b6577df.jpg)

**Enter The Name Of Workspace and click Next.**

![4](https://user-images.githubusercontent.com/119833411/241568066-7c3f8df9-d27c-4980-a3bc-0c947fd288f1.jpg)

**Enter your Name and click Next.**

![5](https://user-images.githubusercontent.com/119833411/241568236-d7b1cebf-0490-4e1c-beb4-6a3685036764.jpg)

**Can Add Team Members To Work on DevOps Workspace or Skip for now.**

![6](https://user-images.githubusercontent.com/119833411/241568413-3a39f5c8-33a9-4abb-a37a-960b0e6d91d6.jpg)

**Enter Channel Name and Click Next.**

![7](https://user-images.githubusercontent.com/119833411/241568601-e86ae169-1460-4d14-bf8e-e6a07be39621.jpg)

**Clich On Lets Go.**

![8](https://user-images.githubusercontent.com/119833411/241568680-fc3cc8a4-9f80-4113-afc3-da6ecd54d9c7.jpg)

**Click The 3-Vertical Dots.**

![9](https://user-images.githubusercontent.com/119833411/241568795-37367ef5-717f-49d7-a626-432634c17094.jpg)

**Select Apps.**

![11](https://user-images.githubusercontent.com/119833411/241568955-c59f68dc-041a-4f20-a610-9854fd496677.jpg)

**Search for Jenkins CI then Add.**

![12](https://user-images.githubusercontent.com/119833411/241569164-4baab19c-cb94-4554-8f9f-67c7c6e9910c.jpg)

**New Tab will Open, Click Add To Slack.**

![13](https://user-images.githubusercontent.com/119833411/241569267-5f88a92f-2e3d-425b-bbf6-149821c7ad43.jpg)

**Choose A Channel Name Where You Want To Get Notifications.**

![14](https://user-images.githubusercontent.com/119833411/241569355-a27516d4-2281-490c-ad6c-68a6790d4ca5.jpg)

**Click Add Jenkins CI Integration.**

![15](https://user-images.githubusercontent.com/119833411/241569451-9461883e-8217-4463-91ba-24ea93587329.jpg)

**You Will Get Set-Up Instructions, Just Follow It.**

![16](https://user-images.githubusercontent.com/119833411/241569612-2efe9963-ef6a-4b27-a755-eabd275f0f0d.jpg)

**In your Jenkins Dashboard, Click on Manage Jenkins.**

![17](https://user-images.githubusercontent.com/119833411/241569861-75163f32-55b1-4c8d-b78c-0bdf5d784bce.jpg)

**Click on Manage plugins and search for Slack notification in the Available tab. Click the tick box and install the plugin.**

![18](https://user-images.githubusercontent.com/119833411/241569987-c96b856b-cfda-415d-a74b-6273d5801251.jpg)

**Once it’s installed, click on Manage Jenkins then go to Configure system.**

![19](https://user-images.githubusercontent.com/119833411/241570143-8eab41fd-c9a2-4a88-aec5-d2ba047286f8.jpg)

**Find the Slack section and add the following values as per Your Set-Up Instructions.**

![20](https://user-images.githubusercontent.com/119833411/241570593-ae0206aa-6ece-4bab-ad96-940e9f4a04bc.jpg)

**Below are My Values as per my Set-Up Instructions**

![16](https://user-images.githubusercontent.com/119833411/241570448-dee3a538-5107-473f-9515-e526d8766bfc.jpg)

**Add Team subdomain value in Workspace then Click on Add and Jenkins.**

![21](https://user-images.githubusercontent.com/119833411/241570848-36d2f570-b308-4a40-92e2-6778086ac5b4.jpg)

**Select Kind to Secret Text.**

![22](https://user-images.githubusercontent.com/119833411/241571116-c7e94762-5bc0-492e-aa6e-1e393624e7f8.jpg)

**Add Integration token credential ID in Secret, Then Add Description and Click Add.**

![24](https://user-images.githubusercontent.com/119833411/241571327-636978a2-a4e9-4514-9783-ea9b0c68261c.jpg)

**Now Click on Credential and Select Your Saved Key.** 

![25](https://user-images.githubusercontent.com/119833411/241571442-6aac1b6e-8970-4021-860f-2814eaa6960d.jpg)

**Click on Test, You Should See Success, Then Click Apply and Save.**

![26](https://user-images.githubusercontent.com/119833411/241571604-f9ad6db2-c353-40d4-9421-cd41ea0a3c24.jpg)

### Integration is Successful, You Can See The url of Jenkins Server.

![27](https://user-images.githubusercontent.com/119833411/241571766-1868fe3c-ff58-4e3a-a90d-68a7d11dfacb.jpg)

### Lets Test By Building a Job on Jenkins.

![28](https://user-images.githubusercontent.com/119833411/241571910-2eeae21f-2c95-426d-bea4-564dbf11d112.jpg)

### Create a Test-Project of Freestyle Project and Click Ok.

![29](https://user-images.githubusercontent.com/119833411/241572046-f0887873-9996-4d96-b801-acaf7d5f9819.jpg)

### Select Build Step. 

![30](https://user-images.githubusercontent.com/119833411/241572172-840e8d29-ffe6-4321-b525-199964f98f62.jpg)

### Select Execute Shell.

![31](https://user-images.githubusercontent.com/119833411/241572266-a9f95cbb-7548-4b74-a943-85c85d2fe272.jpg)

### Enter echo "Hello-World".

![32](https://user-images.githubusercontent.com/119833411/241572728-51d624bd-f869-4f25-a22e-ab7625622241.jpg)

### Go to Post Build Actions, Select Slack Notifications.

![33](https://user-images.githubusercontent.com/119833411/241572814-76b4c53c-0089-4ff1-92af-44c7777a14eb.jpg)

### Select All Available Options, Then Click Apply and Save.

![34](https://user-images.githubusercontent.com/119833411/241572955-961a50e7-b3a2-4aa0-872e-bf5a20a5af86.jpg)

### You Can See No Notifications in Slack.

![36](https://user-images.githubusercontent.com/119833411/241573068-e617e617-dc4f-4912-866e-b0b15fb0e752.jpg)

### Now Click On Build Now.

![35](https://user-images.githubusercontent.com/119833411/241573081-94dc06ea-165e-41d1-98d3-10c82256952e.jpg)

### Build-1 Success.

![37](https://user-images.githubusercontent.com/119833411/241573215-c93177b1-988c-422d-941f-cac68df65f86.jpg)

![38](https://user-images.githubusercontent.com/119833411/241573266-dd51f9ab-8d36-4509-a849-bd28b3ead327.jpg)

### We Can See Build Notifications on Slack.

![39](https://user-images.githubusercontent.com/119833411/241573349-a3b1ca19-d64e-42a7-a79b-6c1c6d4bd07b.jpg)

## We have Successfully Integrated Jenkins Pipeline with Slack Notifications.

**Thank you for reading this post! I hope you found it helpful. If you have any feedback or questions,Please 
connect with me on LinkedIn at https://www.linkedin.com/in/sampathsivakumar-boddeti-1666b810b/. Your feedback is valuable to me. 
Thank you!**























