- After installing Windows Server, we will attempt to navigate to the Active Directory.
- In server manager click on tools and click **Active Directory Users And Computers**.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/aa5a3844-a372-444a-b2d6-7fd8884fafa7)

- **corp.ADLabDelta.com** is a domain controller. A domain controller, in contrast, is simply a server running Active Directory that authenticates users and devices
- When right-clicking corp.ADLabDelta.com, there is an option called `New.` By selecting that option, you will find another choice called **Organizational Unit**.An OU is a container within a Microsoft Windows Active Directory (AD) domain that can hold users, groups and computers. It is the smallest unit to which an administrator can assign Group Policy settings or account permissions.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/4d98eb2d-a61f-4799-8a09-7dc574812714)

An OU here can also be classified as a different geographic location. For example, in your office or company, you may have various global offices or physical locations, and you can name the OU according to the location. For instance, I've named it `India` here.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/f452b5d4-ec21-4a92-b670-7843b7230a68)

So, an OU is essentially a folder that contains various objects like users, groups, devices, and applications. Within an OU, you can create another OU in two ways. The first method is to right-click it and select New. The second method is to highlight the OU, go to the top, and you'll see icons there. You can add different objects such as users and groups. The OU appears as a folder icon, and you can click on it to add another OU using this method.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/b391d8e1-97e3-47aa-a2f4-11a736571966)

Under India, I have created four different OUs, namely Computers, Distribution Groups, Security Groups, and Users.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/ac9350f9-f189-44ec-8ec8-29933189b9d8)

Under Computers, I have created two OUs, one called Server and another one called Workstations.
Under Users, I have grouped them into different departments and created separate OUs for each department, such as Accounting, HR, Engineering, Sales, and Marketing and Termed (for the users that are no longer part of the company)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/7c8b2ea6-ee32-475b-ba0f-cd55f2d18a7c)

Under Security Groups, I have grouped them into different groups, specifically Payroll, IT, Onboarding, Contracts, Sales. 
Active Directory has two types of groups:
- Security groups: Use to assign permissions to shared resources.
- Distribution groups: Use to create email distribution lists.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/a12adc88-4964-4535-8ab3-8b1d33b9dcb8)

The next step I've taken is to create a user within an OU. In the real world, manual entry of user data for employees is not common. Instead, most of the time, user information is automatically populated in Active Directory through scripts to simplify the process for administrators. For training purposes, I have manually added a user. To manually add a user, you can right-click on the user folder, select New, and then choose User. From there, you can fill in all the required information for the user

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/b1f09340-5429-4ae3-8442-063c7ebbda6c)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/efd2ffb9-b420-43c8-bda2-741513afba84)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/49e8580a-aade-4980-827d-98368abddc7f)

Once you've filled in all the required information for the user, click on Finish to complete the user creation process.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/d866071e-46a4-41ca-a351-8cd90ce566de)

If you want to move a user to a different department or group, you can do so by highlighting the user, right-clicking, and selecting the Move option.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/7b133574-bbe8-4874-a471-39f8143bc910)

When you select the Move option and choose the different groups, you can specify where you want to move the user. For instance, if John.P belongs to the Engineering department, you can click on Engineering to move him to that department or group.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/9f89fd6a-e6f9-44f0-96e4-1b93ae1570f7)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/2bb663c1-b200-4c0e-8b6a-f68136bb32ad)

As mentioned earlier, a security group is used to assign permissions to shared resources. To create a security group, you can right-click on the appropriate location such as IT under Security Groups, select "New," and then choose "Group." For example, I have created a group called "Domain Admins" to manage permissions and access to specific resources.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/7dd8c038-30e7-4423-b034-1aee658fb7eb)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/5f8a5ed2-c1b7-419f-b575-12f4e3bd2a40)

To find a user among a large number of users in Active Directory, you can click on the domain (e.g., corp.ADLabDelta.com) that you're using, right-click on it, and select the Find option. Then, you can simply type in the name of the user you're looking for. For example, if you type John.P, John.P will appear in the search results, making it easier to locate the specific user you need.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/b0bc9d6e-5438-41e0-866e-74068f90294c)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/7e284f73-88d0-4b8b-bca9-6e79d6dda7c3)

If you're looking for a specific computer in Active Directory, you can right-click, select Find, change the search category to Computers, and then type in the name of the computer you're searching for. This will help you quickly locate the desired computer object within your directory.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/79e833c2-c4a0-42da-a956-1be9add537d1)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/a9e2c1df-d8ad-435a-b2fa-dc34cde8fa78)

To add various objects to different groups, such as a user like John.P, and include John.P in a group that we've created, go to the Member Of section and click on Add. You can type in the name of the group that you want the user to be a part of 

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/0781d3fd-70ca-47f1-bca7-5d9d364404a1)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/5493bd2c-352f-492a-a1cf-579a923680e5)

We can also enable or disable an account here. For example, if we need to disable John.P's account, we can move the account to the Termed group.Right click on the user and select disable account

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/33d1fdbd-3d29-4aa7-9f3d-e7e986dc1a47)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/c6c1775b-954b-4a9b-91ba-7004427e3198)

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/64c9cad0-24d1-4c59-b208-90a673254b75)

To enable the account, you can check the "Termed" group, right-click on the user, and select Enable Account.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/35d116a9-db63-416d-a221-cefdcb7c1404)

To reset the password, right-click on the user and select Reset Password.

![image](https://github.com/AlphaDeltaGamma/HomeLab-Active-Directory-/assets/92504746/a5326645-2f13-4575-8606-c968f4134c43)




























































































  














































