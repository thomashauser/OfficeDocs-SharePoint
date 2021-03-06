---
title: Plan for OneDrive
ms.author: kaarins
author: kaarins
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: one-drive
localization_priority: Normal
description: "Learn how to plan your OneDrive deployment for an enterprise."
---

# Plan for OneDrive for enterprises

Enterprise deployment guide: Part 2 of 4

This article walks you through the planning and decision points for deploying OneDrive in a corporate or enterprise environment. Read this article before you read Part 3, [Deploy OneDrive](deploy-onedrive-enterprise.md).

Many of the sections in this article list key decisions that you need to make as part of your OneDrive deployment. Make note of each of these decisions for use during the actual deployment process.

## How organizations deploy and manage OneDrive

You can deploy and manage OneDrive in many ways, but certain options make more sense in larger organizations than in smaller businesses and vice versa. For example, it likely wouldn’t make sense to have an enterprise management solution like Microsoft System Center Configuration Manager for a business that has just 10 employees. Table 1 outlines the deployment and management tools typically used for small businesses, medium-sized businesses, and enterprises. 

> [!NOTE]
> Keep in mind that an organization in one size category would probably incorporate additional options from other size categories. This table is not intended to exclusively identify a technology with a specific business size. 

|**Size of organization**|**Deployment tools used**|**Management**|
|:-----|:-----|:-----|
|Small business|Local installation|OneDrive admin center|
|Medium-sized business|Scripted installation or Microsoft Intune mobile device management (MDM)|Office 365 with MDM, OneDrive admin center, Intune mobile application management (MAM) or MDM|
|Enterprise|System Center Configuration Manager with Intune or Windows Autopilot|System Center Configuration Manger, Group Policy objects (GPOs), etc. |

Depending on where your organization fits in this table and the technologies available to you, you can choose which portion of this guide to use. For example, if you run a small businesses, you may want to keep your OneDrive deployment simple by installing the sync client manually on your employees’ computers and using the OneDrive admin center to manage a few settings for your users. Alternatively, if you’re running an enterprise, you may choose to deploy and manage OneDrive by using advanced tools like System Center Configuration Manager and Group Policy, and you could use the sections that correspond to those tools, instead. To accommodate various situations, the deployment and management portions of this guide are in a modular format so that you can consume the document in the way that best aligns with your deployment needs and capabilities. This format also provides visibility into alternate technologies to improve your current processes. 

## Prerequisites

- Client and app requirements. Even though you can upload, download, and interact with your OneDrive files from a web browser, the ideal OneDrive experience comes from the Windows and Mac sync clients and the iOS and Android mobile apps. With that in mind, OneDrive is available for most operating systems and browsers and requires minimal hardware. For a full list of client and app requirements for using OneDrive, see [OneDrive system requirements](https://support.office.com/article/cc0cb2b8-f446-445c-9b52-d3c2627d681e).

- License requirements. There are multiple methods by which you can acquire a license for OneDrive. However, a few OneDrive features are available only within certain licensing models. For information about the licensing requirements for OneDrive, its advanced features, and any special licensing required for them, see [Office 365 plans](https://products.office.com/business/compare-more-office-365-for-business-plans).

## Deployment process

When deploying any new technology, there’s always an ideal process to follow to ensure that you deploy it correctly. This section covers the high-level planning and deployment steps to help ensure that your OneDrive deployment is successful.

> [!NOTE]
> OneDrive deployment can be as simple as a local installation and may not require all the steps in this section. For example, the “Determine devices” and “Align technologies” sections may not be applicable to small business interested in performing a simple installation of OneDrive. 

### Determine devices

Your organization doesn’t have to manage all connected devices for them to use OneDrive, but securing and managing the interaction with the data do require a layer of management capabilities. Start by determining which types of devices—iOS, Android, Windows 10—require access to OneDrive and who owns them (the business or the employee). Put this information in a spreadsheet to help you determine which capabilities you need from your technology solutions. Some management options are more suitable for devices that the company owns and manages. Regardless of the platform running OneDrive and who owns it, the following management options are available to you:

- OneDrive admin center

- Office 365 MDM

- Intune MDM or MAM

For Windows 10 client devices that are joined to a domain, you have the additional option of using GPOs for management. Also, for those devices that are company owned and managed, you can use System Center Configuration Manager to deploy OneDrive.

### Align technologies

When you've identified the devices that require access to OneDrive, you then identify the technology options available to you or that align with your organization’s size. If you’re considering implementing a new deployment and management solution, the table in [How organizations deploy and manage OneDrive](#how-organizations-deploy-and-manage-onedrive) lists the technologies that make the most sense based on organization size. Using this information, you can align the technologies you need or already have with the deployment and management capabilities that fit the devices you need to manage.

### Deploy, secure, and manage OneDrive

You deploy, manage, and secure OneDrive based on the tools you chose in the previous steps. Each technology has different deployment, update, and management options, so when deploying OneDrive, you must first consider whether you need to upgrade existing client machines. Also, securing OneDrive may include both client-side and cloud service–side configuration. Finally, be sure to consider data compliance requirements, such as dedicated storage regions.

## OneDrive limitations

Because OneDrive provides access to files on many kinds of devices, it restricts the use of certain characters, file names, and folder names. In addition, certain features are available only in the Windows operating system. For a full list of these and other limitations of OneDrive, see [Restrictions and limitations when you sync files and folders](https://support.microsoft.com/en-us/help/3125202/restrictions-and-limitations-when-you-sync-files-and-folders).

## Feature releases and requests

If you want to see the functionality currently under development for OneDrive and Office 365, check out the [Office 365 Roadmap](https://products.office.com/business/office-365-roadmap?filters=) or the [Microsoft OneDrive Blog](https://techcommunity.microsoft.com/onedrive). Finally, if you want to request new functionality or vote on great community ideas for OneDrive, visit [OneDrive UserVoice](https://onedrive.uservoice.com).

## Keys to successful user adoption

User adoption is important to the overall success of any new application. Ideally, to feel that you have maximized your investment in Office 365 and OneDrive, you need to maximize user engagement with them. To do that, start by focusing on three critical success factors:

-   **Stakeholders.** Securing the participation and buy-in of key people within your organization is critical to successful user adoption. This support can come from business-focused leaders, IT leadership, or anyone else who has a vested interest in seeing OneDrive and Office 365 succeed in the organization. It is important to have both executive or business leader support and product champions to help carry the knowledge to their peers. Whether you’re formally delegating the product champion role or allowing it to grow organically, champions are mission critical to user adoption. In fact, a SharePoint user study in 2013 showed that people prefer to learn from a coworker than from an IT employee. For more information about how to identify key stakeholders for your OneDrive and Office 365 implementation, see the [Identify key stakeholders guide](https://aka.ms/execsponsor). For more information about building a sustainable champion community, see [Build a champion program](https://aka.ms/office365champions).

-   **Scenarios.** When planning to implement OneDrive and Office 365, identify and define your business scenarios and how those scenarios align with the benefits of implementing OneDrive and Office 365. Work with your key stakeholders to identify the goals of the business scenarios, and then match those goals against usage scenarios. For example, a business goal may be to maximize user productivity; a key usage scenario enabling that goal would be using OneDrive to access files from mobile devices, PCs, and Macs. For help with this process, see the [Office 365 Productivity Library](https://www.microsoft.com/microsoft-365/success/?rtc=1).

-   **Awareness and training.** Creating awareness through awareness campaigns such as announcements, launch events, newsletters, town hall meetings, contests, and giveaways is a critical path to maximizing adoption. In addition, providing users with knowledge through classroom-style sessions and self-help guides helps them feel empowered to use OneDrive and Office 365. For more information about user communication and training on Office 365, see the [Plan your Office 365 Launch: Communication and Training Guide](https://aka.ms/commandtraining).

Many resources are available from Microsoft to help you drive user adoption within your environment. For more information about a recommended Microsoft 365 user adoption strategy, see the [Microsoft 365 End User Adoption Guide](https://fto365dev.blob.core.windows.net/media/Default/DocResources/en-us/Microsoft%20365%20User%20Adoption%20Guide.pdf). For more information about driving user engagement, see [Success Factors for Office 365 End User Engagement](https://fto365dev.blob.core.windows.net/media/Default/DocResources/en-us/Resources/Office365_AdoptionBrochure_v2.0_Screen.pdf). You can also contribute to or comment on adoption-related ideas in the [Driving Adoption Tech Community](https://techcommunity.microsoft.com/t5/Driving-Adoption/ct-p/DrivingAdoption).

## Preparing your environment

Before you deploy OneDrive, prepare your environment.

### Network utilization

A variety of factors can impact the amount of network bandwidth used by OneDrive. For the best experience, we recommend that you assess this impact before doing a full OneDrive deployment across your organization. The article [Network utilization planning for the OneDrive sync client](network-utilization-planning.md) includes the recommended process for determining your network bandwidth needs for OneDrive. Be sure to include this as part of your deployment plan.

### Multi-Geo

If you have data residency requirements, consider OneDrive Multi-Geo. With OneDrive Multi-Geo, you can specify a preferred data location (PDL), from available locations around the world, for each user’s OneDrive. For detailed information about OneDrive Multi-Geo, see [Multi-Geo Capabilities in OneDrive and SharePoint Online in Office 365](/office365/enterprise/multi-geo-capabilities-in-onedrive-and-sharepoint-online-in-office-365.md).

If you plan to deploy OneDrive Multi-Geo, there are two user scenarios:

-   Users who start using OneDrive before you configure OneDrive Multi-Geo – their OneDrive will be located in the central location once you configure OneDrive Multi-Geo. If you need to move a user's OneDrive to a different geo location, follow the steps in [Move a OneDrive site to a different geo-location](/office365/enterprise/move-onedrive-between-geo-locations.md) to the.

-   Users who start using OneDrive after you configure OneDrive Multi-Geo – you can configure their preferred data location as part of your general user onboarding process and their OneDrive will be created in the appropriate geo location.

Features such as file sync and mobile device management work normally in a multi-geo environment. There’s no special configuration or management needed. The multi-geo experience for your users has minimal difference from a single-geo configuration. See [User experience in a multi-geo environment](/office365/enterprise/multi-geo-user-experience.md) for details.

If you plan to configure OneDrive Multi-Geo prior to deploying OneDrive for your users, read [Plan for OneDrive for Business Multi-Geo](https://docs.microsoft.com/office365/enterprise/plan-for-multi-geo) and follow the steps in [OneDrive for Business Multi-Geo tenant configuration](https://docs.microsoft.com/office365/enterprise/multi-geo-tenant-configuration).

Key decisions:

-   Do you plan to use OneDrive Multi-Geo?

-   Will you have OneDrive Multi-Geo fully configured before your users start using OneDrive?

### Hybrid

If you currently use OneDrive or MySites in SharePoint Server on-premises, we highly recommend deploying hybrid OneDrive. With hybrid OneDrive, users are redirected from their on-premises OneDrive to OneDrive in Office 365. Hybrid OneDrive allows for seamless navigation to OneDrive in the cloud from both SharePoint on-premises and Office 365.

When you deploy hybrid OneDrive, the OneDrive links in the SharePoint Server ribbon and app launcher will point to OneDrive in Office 365. If your users have files in on-premises OneDrive, they may have trouble accessing them unless they’ve bookmarked the old URL. It’s important to have a migration plan for these files before you deploy hybrid OneDrive. See [Migrating data](#migrating-data) later in this article for migration options.

If you don’t use OneDrive in SharePoint Server, but you do have an on-premises SharePoint environment, you may still want to consider deploying hybrid OneDrive. Doing so will update the OneDrive navigation links in SharePoint Server to point to OneDrive in Office 365 – again, giving your users seamless navigation to OneDrive in the cloud from either location.

For more information about how to configure OneDrive in a hybrid scenario and how it works, see [Plan hybrid OneDrive for Business](/hybrid/plan-hybrid-onedrive-for-business.md).

SharePoint hybrid has a variety of features to create a seamless experience when using both SharePoint Server and SharePoint Online. If you’re planning to configure hybrid OneDrive, consider including other SharePoint hybrid features for a better overall user experience. See [Explore SharePoint Server hybrid](/hybrid/explore-sharepoint-server-hybrid.md) for more information.

Once you’ve migrated your users’ files from on-premises OneDrive and configured hybrid OneDrive, you can reduce the quota for your on-premises OneDrive top-level site collection to a minimal value to save disk space.

Key decisions:

-   Do you want to deploy hybrid OneDrive?

-   Do your users have OneDrive on-premises data that needs to be migrated to OneDrive in Office 365?

## Access and sharing considerations

OneDrive shares can contain sensitive information that could damage your organization if it were shared with the wrong people. This section provides information about how to help prevent accidental data leakage and protect your data by controlling who can access it.

### Information rights management–protected file synchronization

If you’re using information rights management (IRM), OneDrive can synchronize those file libraries and provide a seamless experience for users. For detailed information about how OneDrive handles IRM, see [How Office applications and services support Azure Rights Management](/information-protection/understand-explore/office-apps-services-support.md). For OneDrive to synchronize these IRM-protected libraries, however, additional configuration is required, including deploying the latest [Rights Management Services (RMS) client](https://www.microsoft.com/en-us/download/details.aspx?id=38396) to your users’ computers. For details about the additional configuration required for OneDrive to support IRM libraries, see [SharePoint Online and OneDrive for Business: IRM Configuration](/information-protection/deploy-use/configure-office365#sharepoint-online-and-onedrive-for-business-irm-configuration.md).

### Windows Information Protection

You can use Windows Information Protection (WIP) to help prevent data leakage by deploying application or device policies that restrict how your employees can store, access, and use your organization's data. For example, you can restrict users to synchronizing files that contain company data only to OneDrive and not to personal cloud storage providers like Dropbox. For information about how to use WIP, see [Protect your enterprise data using Windows Information Protection (WIP)](/windows/security/information-protection/windows-information-protection/protect-enterprise-data-using-wip.md).

If you’ve decided to use Windows Information Protection with OneDrive, see the following resources to set up your Windows Information Protection policies:

-   [Create a Windows Information Protection (WIP) policy using Microsoft Intune](https://docs.microsoft.com/windows/security/information-protection/windows-information-protection/overview-create-wip-policy)

-   [Create a Windows Information Protection (WIP) policy using System Center Configuration Manager](https://docs.microsoft.com/windows/security/information-protection/windows-information-protection/overview-create-wip-policy-sccm)

Key decision:

-   Do you want to user Windows Information Protection with OneDrive?

### Azure Information Protection

Azure Information Protection is a cloud-based solution that helps organizations classify, label, and protect their documents and emails. This classification can occur automatically when administrators define rules and conditions; manually by users; or both, where users receive recommendations. Users can synchronize Azure Information Protection–protected files to OneDrive after you have configured their accounts to do so.

For more information about Azure Information Protection, see [What is Azure Information Protection](/azure/information-protection/understand-explore/what-is-information-protection.md)? You can add Azure Information Protection to your Office 365 subscription through the Billing\\Subscriptions section of the [Admin Center](https://portal.office.com/adminportal/home#/homepage).

If you have decided to use Azure Information Protection, see [Office 365: Configuration for clients and online services to use the Azure Rights Management service](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-office365#sharepoint-online-and-onedrive-for-business-irm-configuration)[](https://docs.microsoft.com/information-protection/deploy-use/configure-office365#sharepoint-online-and-onedrive-for-business-irm-configuration) to configure the necessary settings for it to work with OneDrive.

### Sharing options

Using the OneDrive admin center, you can specify sharing options such as the default sharing type for users, with whom they can share, and how long sharing links remain active.

These are the key decisions around sharing for OneDrive:

-   **Do you want to allow external sharing?** If you enable external sharing for OneDrive, your users will be able to share files and folders with people outside your organization.

-   **If you allow external sharing, do you want to allow unauthenticated users?** If you enable sharing with **Anyone**, users can create sharable links that don’t require sign-in.

-   **What do you want the default sharing link to be?** Users can choose which type of link to send (Anyone, Internal, or Direct), but you can choose the default option that is presented to users.

-   **Do you want to restrict external sharing by domain?** You can restrict external sharing to specific domains or prevent sharing with specific domains.

Note that the OneDrive sharing settings are a subset of the SharePoint Online sharing settings. If you want to allow external sharing in OneDrive, it must be enabled for SharePoint Online.

### OneDrive integration with other Office 365 features

OneDrive integrates with many other applications, such as SharePoint, Teams, and Yammer. With that integration comes the necessity to protect the data stored in OneDrive. When considering security, for example, think about potential leakage scenarios through each integrated application and apply WIP, IRM, Azure Information Protection, or another protection option to help prevent unauthorized access. For information about how these products integrate with each other to provide a better collaboration solution and how they can introduce additional vectors for data leakage, see [How SharePoint Online and OneDrive for Business interact with Microsoft Teams](/microsoftteams/sharepoint-onedrive-interact.md).

### Data retention

When a user leaves your organization and you’ve deleted that user’s account, what happens to his or her data? When considering data retention compliance, determine what needs to happen with the deleted user’s data. For some organizations, retaining deleted user data could be important continuity and preventing critical data loss. The default retention policy for deleted OneDrive users is 30 days. You can configure the setting to a range between 0 days and 3,650 days (ten years).

For more information about OneDrive retention, see [OneDrive retention and deletion](retention-and-deletion.md) and [Overview of document deletion policies](https://support.office.com/article/55e8d858-f278-482b-a198-2e62d6a2e6e5).

Key decision:

-   What data retention time do you need for your organization?

## Migrating data

A key task in deploying OneDrive for your organization is a plan to migrate your users existing files to OneDrive. Depending on where these files are kept, there are several options, discussed below. You can choose one or more of these options depending on the number and location of files that you need to migrate.

Another planning consideration is who will be migrating the data. Normally, a user’s OneDrive is created the first time they access OneDrive. If you will be migrating your users’ files on their behalf before they begin using OneDrive, you may need to pre-provision OneDrive for each of them. (This can be done with a PowerShell script.)

Keep in mind that any of the migration options listed below may result in a surge of network activity as large numbers of files are migrated to OneDrive.

Key decisions:

-   Which of the following migration methods do you want to use?

-   Are you configuring hybrid OneDrive? (See the hybrid section of this article for the considerations around this option.)

-   Do you need to pre-provision OneDrive for your users? (Are you migrating files before users have started using OneDrive?)


### Files in on-premises OneDrive or MySites libraries

If users' existing files are in on-premises SharePoint, OneDrive, or MySites, you can use the SharePoint Migration Tool to migrate the files to Office 365.

For detailed information about the SharePoint Migration Tool, see [How the SharePoint Migration Tool works](/sharepointmigration/how-the-sharepoint-migration-tool-works.md).

The SharePoint Migration Tool can be used by your IT department to migrate files on their behalf. This is the reocmmended method of migration for files in an on-premises SharePoint farm.


### Files on users' local disk in known folders

If user files are located in Windows known folders such as their desktop, Documents, or Pictures, you can use Known Folder Move. Known Folder Move enables users to select known folders to automatically synchronize to OneDrive. You can add this feature during the initial setup of OneDrive or after it has been configured. This capability provides a simple migration option for users looking to add known folders to their existing list of synchronized folders.

Known Folder Move can be configured by administrators to automatically redirect known folders for all users on the domain. It's an easy way to migrate files kept in these locations.

### Files in other local disk folders

If users have their additional work files in various locations on their computers, it's often easiest for them to manually move the files to OneDrive. After you deploy the OneDrive sync client to your users' computers, you can instruct them to move their work files to the OneDrive folder on their computer.

### Migrating with FastTrack

FastTrack is a Microsoft benefit that is included in your subscription.  FastTrack provides you with a set of best practices, tools, resources, and experts committed to making your experience with the Microsoft Cloud a great one! Guidance around OneDrive onboarding, migration, and adoption are included in the benefit offering. This guidance includes: help to discover what’s possible, creating a plan for success, and onboarding new users, providing guidance on migrating content from file share, Box, or Google Drive source environments, and introducing capabilities at a flexible pace, your pace! FastTrack guidance provides enablement of both OneDrive for Business and getting the source environment ready for your transition. In addition, the FastTrack data migration benefit will also perform specific data migration activities on behalf of you, the customer,  for those with 500 or more licenses. See more details in the provided [FastTrack Center Benefit Overview](/fasttrack/fasttrack-benefit-for-office-365/fasttrack-benefit-overview/data-migration.md). Interested in getting started? Visit [FastTrack.Microsoft.Com](https://www.microsoft.com/en-us/fasttrack/), review resources, and submit a Request for Assistance.

## Sync

Even though you can upload, download, and interact with your OneDrive files from a web browser, the ideal OneDrive experience comes from the Windows and Mac sync clients and the iOS and Android mobile apps. OneDrive is available for most operating systems and browsers and requires minimal hardware. For a full list of client and app requirements for using OneDrive, see [OneDrive system requirements](https://support.office.com/article/cc0cb2b8-f446-445c-9b52-d3c2627d681e).

If you already have the OneDrive client installed on Windows devices, start by determining the version or versions of OneDrive in your environment. Depending on your findings, you may need to change your deployment process to accommodate the current version (for example, run takeover commands in PowerShell to ensure that data sync responsibilities transition to the new client). To determine which version of OneDrive you’re currently using, see [Which version of OneDrive am I using?](https://support.office.com/article/19246eae-8a51-490a-8d97-a645c151f2ba)


### Upgrade from the Groove sync client to the OneDrive sync client

If you currently have the old OneDrive sync client (Groove.exe), then you’ll need to follow a slightly different process to upgrade to the new sync client. If you had more than 250 licensed users before June 2016, you may need to run a takeover command to continue syncing existing libraries using the new client. For detailed information about this process (and caveats), see [Transition from the previous OneDrive for business sync client](transition-from-previous-sync-client.md).

### Sync client update process

You can update the OneDrive sync client in two waves:

-   **Production ring** – in this ring, you get new features and improvements sooner – as soon as they’ve been validated within Microsoft.

-   **Enterprise ring** – in this ring, changes are rolled out after they’ve been validated in the Production ring, reducing the risk of issues.

This setting is configured by using group policy.

For details about the update process for the OneDrive sync client, see [The OneDrive sync client update process](sync-client-update-process.md).

To find out about new features available in current OneDrive updates as well as the current and historical version numbers, see [New OneDrive sync client release notes](https://support.office.com/article/845dcf18-f921-435e-bf28-4e24b95e5fc0).

Key decision:

-   Which ring do you want to use for updates to the OneDrive sync client?

### Deploying OneDrive in your organization

Once you have made the key decisions regarding your OneDrive deployment, go on to Part 2, [Deploy OneDrive](deploy-onedrive-enterprise.md) for specific steps that guide you through the deployment process.
