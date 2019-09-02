---
title: "About admin roles in the Microsoft 365 admin center"
ms.author: anfowler
author: adefowler
manager: shohara
audience: Admin
ms.topic: overview
f1_keywords:
- 'O365P_AssignAdminRoles'
- 'O365M_AssignAdminRoles'
- 'O365E_AssignAdminRoles'
ms.service: o365-administration
localization_priority: Normal
ms.collection: 
- M365-subscription-management
- Adm_O365
- Adm_TOC
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: da585eea-f576-4f55-a1e0-87090b6aaa9d
description: "Admin roles map to business functions and give permissions to do specific tasks in the admin center. For example, the Service admin opens support tickets with Microsoft.."
---

# About admin roles


Your subscription comes with a set of admin roles that you can assign to users in your organization. Each admin role maps to common business functions and gives people in your organization permissions to do specific tasks in the admin centers. For more information, see [Assign admin roles](assign-admin-roles.md)

[!TIP] Looking for the detailed role descriptions? Check out [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

## Things to consider...

Because admins have access to sensitive data and files, we recommend that you follow these guidelines to keep your organization's data more secure.

| Recommendation                  | Why is this important?                 |
| :------------------- | :------------------- |
| Have 2 to 4 global admins  | Because only another global admin can reset a global admin's password, we recommend that you have at least 2 global admins in your organization in case of account lockout. But the global admin has almost unlimited access to your org's settings and most of the data, so we also recommend that you don't have more than 4 global admins because that's a security threat. |
| Assign the *least permissive* role    | Assigning the *least permissive* role means giving admins only the access they need to get the job done. For example, if you want someone to reset employee passwords you shouldn't assign the unlimited global admin role, you should assign a limited admin role, like Password admin or Helpdesk admin.  This will help keep your data secure.                 |
| Require multi-factor authentication for admins                  |    It's actually a good idea to require MFA for all of your users, but admins should definitely be required to use MFA to sign in. MFA makes users enter a second method of identification to verify they are who they say they are. Admins can have access to a lot of customer and employee data and if you require MFA, even if the admin's password gets compromised, the password is useless without the second form of identification.  <br><br>When you turn on MFA, the next time the user signs in, they'll need to provide an alternate email address and phone number for account recovery.  <br> [Set up multi-factor authentication](../security-and-compliance/set-up-multi-factor-authentication.md)          | 
## Need more details about what these roles can and cannot do?

You can view the brief descriptions later in this article: [Roles available in the Microsoft 365 admin center](#roles-available-in-the-microsoft-365-admin-center).

If you’re looking for detailed information, including the cmdlets associated with a role, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

But if you have access to the new admin center and the new roles experience is available to you, go to **Roles** > **Roles**, and then select any role to open its detail pane. Select the **Permissions** tab to view the detailed list of what admins assigned that role have permission to do.
  
## Some roles are missing from Active users > Manage admin roles. Where did they go?
By default, we first show roles that most organizations use. If you can't find a role, go to the bottom of the list and select **See more roles**.

## How can I tell which permissions are assigned to me?
If you get a message in the admin center telling you that you don't have permissions to edit a setting or page, it's because you are assigned a role that doesn't have that permission.

## What about the Azure Active Directory roles?

The Azure portal has more roles than available in the Microsoft 365 admin center. If you have a large business, there might be roles in the Azure portal that meet your organizational needs.

For a list and description of all the Azure Active Directory roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

A user who is assigned an admin role will have the same level of access to cloud services that your organization has subscribed to, regardless of whether you assign the role in the Microsoft 365 admin center or the Azure portal, or by using the Azure AD module for Windows PowerShell.
  
## Roles available in the Microsoft 365 admin center

The Microsoft 365 admin center lets you manage over 30 Azure AD roles. However, these roles are a subset of the roles available in the Azure portal.

You'll probably only need to assign the following roles in your organization.

|Admin role     |Who should be assigned this role?  |
|---------|---------|
|Global admin     |   Assign the Global admin role to users who need global access to most management features and data across Microsoft online services. <br><br> Giving too many users global access is a security risk and we recommend that you have between 2 and 4 Global admins. <br><br> Only global admins can:<br> - Reset passwords for all users <br> - Add and manage domains <br> <br> **Note:**   The person who signed up for Microsoft online services automatically becomes a Global admin. |
|Billing admin     |    Assign the billing admin role to users who need to do the following:<br>- Purchase subscriptions and licences <br> - Upgrade subscriptions <br> - Pay for services <br> - Receive email notifications for invoices <br> - Manage service requests <br> - Monitor service health   |
|Helpdesk admin     |   Assign the Helpdesk admin role to users who need to do the following:<br> - Rest passwords <br> - Force users to sign out <br> - Manage service requests <br> - Monitor service health <br> <br> **Note**: The Helpdesk admin can only help non-admin users and users assigned these roles: Directory reader, Guest inviter, Helpdesk admin, Message center reader, and Reports reader.      |
|License admin     |     Assign the license admin role to users who need to do the following: <br> - Manage licenses assigned to users <br> - Manage licenses assigned to groups using group-based licensing.<br> - Edit usage location for users<br><br> **Note**: This role doesn't give permission to purchase or manage subscriptions, add or manage groups, or edit user properties, except for usage location.  |
|Reports reader     |   Assign the reports reader role to users who need to do the following: <br> - View usage data and activity reports<br> - Access Power BI adoption content pack <br> - View sign-in reports and activity <br> - View data returned by Microsoft Graph reporting API      |
|User admin     |    Assign the User admin role to users who need to do the following for all users: <br> - Add users and groups <br> - Assign licenses <br> - Manage most users properties <br> - Create and manage user views <br> - Update password expiration policies <br> - Manage service requests <br> - Monitor service health <br><br>  The user admin can also do the following actions for users who aren't admins and for users assigned the following roles: Directory reader, Guest inviter, Helpdesk admin, Message center reader, Reports reader: <br> - Manage usernames<br> - Delete and restore users<br> - Reset passwords <br> - Force users to sign out <br> - Update (FIDO) device keys   |

### All roles

 Here's a list of all the roles available in the Microsoft 365 admin center.

|Role     |Description  |
|---------|---------|
|Application admin     |    Full access to enterprise applications, application registrations, and application proxy settings.     |
|Application developer     |    Create application registrations and consent to app access on their own behalf.     |
|Authentication admin     |    Can require users to re-register authentication for non-password credentials, like MFA.     |
|Azure Information Protection admin     |   Manages labels for the Azure Information Protection policy, manages protection templates, and activates protection.       |
|Billing admin     |    Makes purchases, manages subscriptions, manages service requests, and monitors service health.     |
|Cloud application admin     | Full access to enterprise applications and application registrations. No application proxy.     |
|Cloud device admin     |    Enables, disables, and deletes devices and can read Windows 10 BitLocker keys.     |
|Compliance admin     |    Manages regulatory requirements and eDiscovery cases, maintains data governance for locations, identities, and apps.     |
|Conditional Access admin     |   Manages Azure Active Directory conditional access settings, but not Exchange ActiveSync conditional access policy.      |
|Customer Lockbox access approver     |      Manages Customer Lockbox requests, can turn Customer Lockbox on or off.   |
|Desktop Analytics admin     |   Can access and manage Desktop management tools and services.      |
|Dynamics 365 admin     |  Full access to Microsoft Dynamics 365 Online, manages service requests, monitors service health.       |
|Exchange admin     |  Full access to Exchange Online, creates and manages groups, manages service requests, and monitors service health.    |
|External identity provider admin    |     Configure identity providers for use in direct federation.    |
|Global admin     |    Has unlimited access to all management features and most data in all admin centers.     |
|Guest inviter     |    Manages Azure Active Directory B2B guest user invitations.     |
|Helpdesk admin     | Resets passwords and re-authenticates for all non-admins and some admin roles, manages service requests, and monitors service health.      |
|Kaizala admin     |    Full access to all Kaizala management features and data, manages service requests.     |
|License admin     |     Assigns and removes licenses from users and edits their usage location.    |
|Message center privacy reader     |    Access to data privacy messages in Message Center, gets email notifications.     |
|Message center reader     | Reads and shares regular messages in Message Center, gets weekly email digests, has read-only access to users, groups, domains, and subscriptions.     |
|Privileged role admin     |    Manages role assignments in manages all access control features of Privileged Identity Management.     |
|Reports reader     |   Reads usage reporting data from the reports dashboard, PowerBI adoption content pack, sign-in reports, and Microsoft Graph reporting API.      |
|Search admin     |    Full access to Microsoft Search, assigns the Search admin and Search editor roles, manages editorial content, monitors service health, and creates service requests.     |
|Search editor     |    Can only create, edit, and delete content for Microsoft Search, like bookmarks, Q&A, and locations.     |
|Service admin     |    Creates service requests for Azure, Microsoft 365, and Office 365 services, and monitors service health.     |
|Skype for Business admin     | Full access to all Teams and Skype features, Skype user attributes, manages service requests, and monitors service health.      |
|SharePoint admin     |    Full access to SharePoint Online, manages service requests, and monitors service health.     |
|Teams admin     |    Full access to Teams & Skype admin center, manages service requests, and monitors service health.     |
|Teams communication manager     |    Assigns telephone numbers, creates and manages voice and meeting policies, and reads call analytics.     |
|Teams communication support engineer     |    Reads call record details for all call participants to troubleshoot communication issues.     |
|Teams communication support specialist     |    Reads user call details only for a specific user to troubleshoot communication issues.|
|User admin     |   Resets user passwords, creates and manages users and groups, including filters, manages service requests, and monitors service health.|

## Delegated administration for Microsoft Partners

If you're working with a Microsoft partner, you can assign them admin roles. They, in turn, can assign users in your company - or their company - admin roles. You might want them to do this, for example, if they are setting up and managing your online organization for you.
  
A partner can assign these roles:
  
- Full administration, which has privileges equivalent to a global admin, with the exception of managing multi-factor authentication through the Partner Center.
    
- Limited administration, which has privileges equivalent to a helpdesk admin.

Before the partner can assign these roles to users, you must add the partner as a delegated admin to your account. This process is initiated by an authorized partner. The partner sends you an email to ask you if you want to give them permission to act as a delegated admin. For instructions, see [Authorize or remove partner relationships](https://support.office.com/article/201ccb3b-6011-4bf1-a6b2-84e7cc1ee2d0.aspx).
  
## Related articles

[Assign admin roles](assign-admin-roles.md)
  
[Activity reports in the Microsoft 365 admin center](../activity-reports/activity-reports.md)
