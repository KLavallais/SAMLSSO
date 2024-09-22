# SAML Application Demonstration: Setting Up SSO for 15Five

## Overview
This guide outlines the steps to configure Single Sign-On (SSO) for 15Five using SAML through **Azure Active Directory (Azure AD)**. It also includes assigning users and groups, testing the connection, and customizing the application.

## Video Demonstration
[![SAML SSO Setup](https://github.com/KLavallais/KLavallais/blob/424fbdb6b3348a86979918566f6ea36c04643490/images/SAML%20SSO%20Thumbnail%200002.png)](https://www.youtube.com/watch?v=pXALTU34eMg)

Click the image above to watch a video tutorial on setting up SSO for 15Five.

## Steps:

1. **Start at Enterprise Applications Overview Page**
   - Navigate to the **Enterprise Applications** section in the Azure AD portal.
   - Click on **Overview**.

2. **Create a New Application**
   - Click on **New Application**.
   - Select **Create your own application**.

3. **Name the Application**
   - In the name field, enter **15five2** (or any other preferred name).
   - Ensure that the option **Integrate any other application you don’t find in the gallery** is selected.
   - Click **Create**.

4. **Configure SSO**
   - Once the application is created, you’ll be directed to the application overview page.
   - Click on **Set up single sign on** (option 2).
   - Select **SAML** as the sign-on method.

5. **Configure Basic SAML Settings**
   - At this point, you’ll see the **Basic SAML Configuration** section on Azure AD.
   - Now, switch to the 15Five website to gather necessary information.

6. **Retrieve Service Provider (SP) Information from 15Five**
   - On the 15Five website, click the **gear icon** to open the settings menu.
   - Navigate to **Company settings** > **SSO**.
   - Scroll down to the **Service Provider (SP) Information** section.
   - Copy the information you need from 15Five, including the **ACS URL**, **Entity ID**, and others.

7. **Paste SP Information in Azure AD**
   - Go back to Azure AD, and in the **Basic SAML Configuration** section, paste the copied Service Provider information from 15Five.
   - Click **Save** once you’ve filled in all the fields.

8. **Download Metadata from Azure AD**
   - Scroll down to the **SAML Certificates** section (section 3).
   - Click on the third download option to download the **Federation Metadata XML**.

9. **Upload Metadata to 15Five**
   - Return to the 15Five website.
   - Under **Single Sign-On** > **Metadata & Contact**, upload the **Federation Metadata XML** file you downloaded from Azure AD.

10. **Test the Connection**
    - Go back to Azure AD.
    - Test the SSO connection by clicking the **Test Connection** button.

11. **Assign Users to the Application**
    - Navigate back to the application overview in Azure AD.
    - Click on **Assign users & groups**.
    - Assign individual users to the application.

12. **Assign Groups to the Application**
    - After assigning users, repeat the process by selecting **Groups** instead of individual users.
    - Assign the appropriate group to the application.

13. **Show Assigned Users and Groups**
    - Confirm the users and groups you’ve selected.
    - You can display both the users and groups that are assigned to the application.

14. **Access the App via MyApps**
    - To demonstrate how users can access the application, go to **myapps.microsoft.com**.
    - This portal shows the list of applications available to users after SSO setup.

15. **Customize App Properties**
    - Go back to the **Overview** section of the application in Azure AD.
    - Click on **Properties** to show options for customizing the **logo/icon** of the application.

16. **Remove the Application**
    - To delete the application, select the **Delete** option in the **Overview** section of Azure AD.

## Conclusion
With these steps, you have successfully set up SSO for 15Five using SAML in Azure AD, assigned users and groups, and tested the connection. You can also customize and remove the app as needed.

