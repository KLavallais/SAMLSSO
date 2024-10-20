# SAML Application Demonstration: Setting Up SSO for 15Five
![Microsoft Azure Banner](https://github.com/KLavallais/KLavallais/blob/assets/Microsoft-Azure-Banner_0002.jpg?raw=true)

## Overview

This guide outlines the steps to configure Single Sign-On (SSO) for 15Five using SAML through **Azure Active Directory (Azure AD)**. It also includes assigning users and groups, testing the connection, and customizing the application.

---
### **Tools Used:**
1. **Microsoft Azure Active Directory (Azure AD)**: Used to create and configure applications, assign users/groups, and manage single sign-on (SSO) functionality.
2. **15Five Platform**: The application platform integrated with Azure AD for SSO.
3. **SAML (Security Assertion Markup Language)**: Used to configure the SSO between Azure AD and 15Five.
4. **Azure AD Metadata**: XML metadata used to complete the SSO configuration in 15Five.
5. **My Apps Portal (myapps.microsoft.com)**: The web portal where users can access the applications they have permissions for after SSO is set up.
6. **Company Settings in 15Five**: Interface for configuring SSO settings in the 15Five platform.
7. **SSO Configuration (Single Sign-On)**: Configuration within both Azure AD and 15Five for SSO integration.
8. **User and Group Management in Azure AD**: Used to assign users and groups to the newly created application.

---

### **Skills Displayed:**
1. **Application Creation in Azure AD**: Demonstrated the creation of an application within Azure Active Directory for SSO configuration.
2. **Single Sign-On (SSO) Setup**: Configured SSO using **SAML** between Azure AD and the 15Five platform, including copying metadata and managing settings on both platforms.
3. **Managing Users and Groups in Azure AD**: Assigned individual users and groups (like Help Desk) to the application, ensuring proper access control.
4. **SSO Metadata Configuration**: Downloaded and applied XML metadata to configure SSO, showing the ability to manage detailed configurations.
5. **User Access Management**: Demonstrated how to assign and manage user permissions both individually and via groups for application access.
6. **Azure AD Portal Navigation**: Effectively navigated through the Azure AD portal to set up SSO, assign users/groups, and manage the application.
7. **Application Testing & Overview**: Verified that the application was successfully set up by demonstrating how to access it through the **My Apps Portal**.
8. **Customizing Application Properties**: Mentioned the ability to customize the app by uploading icons or logos and managing application settings (such as deleting the app).


## Video Demonstration
[![SAML SSO Setup](https://github.com/KLavallais/KLavallais/blob/assets/SAML%20SSO%20Thumbnail%200002.png)](https://youtu.be/g96YmnnimfY)

Click the image above to watch a video tutorial on setting up SSO for 15Five.

## Steps:

1. **Start at Enterprise Applications Overview Page**
   - Navigate to the **Enterprise Applications** section in the Azure AD portal.
   - Click on **Overview**.

2. **Create a New Application**
   - Click on **New Application**.
   - Select **Create your own application**.

3. **Name the Application**
   - In the name field, enter **15Five2** (or any other preferred name).
   - Ensure that the option **Integrate any other application you don’t find in the gallery** is selected.
   - Click **Create**.

4. **Configure SSO**
   - Once the application is created, you’ll be directed to the application overview page.
   - Click on **Set up single sign on** (option 2).
   - Select **SAML** as the sign-on method.

5. **Configure Basic SAML Settings**
   - You will see the **Basic SAML Configuration** section in Azure AD.
   - Now, switch to the **15Five** website to gather the necessary information.

6. **Retrieve Service Provider (SP) Information from 15Five**
   - On the **15Five** website, click the **gear icon** to open the settings menu.
   - Navigate to **Company settings** > **SSO**.
   - Scroll down to the **Service Provider (SP) Information** section.
   - Copy the **ACS URL**, **Entity ID**, and any other required values.

7. **Paste SP Information in Azure AD**
   - Return to Azure AD, and in the **Basic SAML Configuration** section, paste the copied Service Provider information from 15Five.
   - Click **Save** once all required fields are filled in.

8. **Download Metadata from Azure AD**
   - Scroll down to the **SAML Certificates** section (section 3).
   - Click on the third download option to download the **Federation Metadata XML**.

9. **Upload Metadata to 15Five**
   - Return to the **15Five** website.
   - Under **Single Sign-On** > **Metadata & Contact**, upload the **Federation Metadata XML** file that you downloaded from Azure AD.
   - Click **Save** after uploading.

10. **Test the Connection**
    - Go back to Azure AD.
    - Test the SSO connection by clicking the **Test Connection** button.
    - Verify that everything works as expected.

11. **Assign Users to the Application**
    - Navigate back to the application overview in Azure AD.
    - Click on **Assign users & groups**.
    - Assign individual users (such as yourself and other specific users) to the application.

12. **Assign Groups to the Application**
    - After assigning individual users, repeat the process by selecting **Groups**.
    - Assign the appropriate group (e.g., **Help Desk**) to the application to give access to all group members.

13. **Show Assigned Users and Groups**
    - Confirm the users and groups you’ve selected.
    - Review and display both the users and groups that are assigned to the application.

14. **Access the App via MyApps**
    - To demonstrate how users can access the application, go to **myapps.microsoft.com**.
    - This portal will display the applications available to users after SSO setup.
    - Ensure **15Five** is listed and accessible.

15. **Customize App Properties**
    - Go back to the **Overview** section of the application in Azure AD.
    - Click on **Properties** to show options for customizing the **logo/icon** of the application (e.g., changing the 15Five app icon).

16. **Remove the Application**
    - If needed, to delete the application, select the **Delete** option in the **Overview** section of Azure AD.
    - This will remove the 15Five application from Azure AD.

---

### Conclusion:
With these steps, you have successfully set up SSO for **15Five** using **SAML** in **Azure AD**, assigned users and groups, and tested the connection. Additionally, you can customize the application’s properties or remove the app as needed.


