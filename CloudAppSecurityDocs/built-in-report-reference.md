---
# required metadata

title: Built-in report reference | Microsoft Docs
description: This topic provides a list of built-in reports and their uses.
keywords:
author: rkarlin
ms.author: rkarlin
manager: mbaldwin
ms.date: 10/15/2016
ms.topic: article
ms.prod:
ms.service: cloud-app-security
ms.technology:
ms.assetid: 588b3639-f748-45a6-bc4b-a6ee47c1865e

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: reutam
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Built-in report reference
It is recommended that you create custom reports using built-in reports as a starting place, sort of like a template on which to base your custom reports. The following table provides a list of built-in reports and the types of events you might want to use them to monitor.  
  
## Built-in report list  
  
|Report type|Built-in report name|Description|  
|-----------------|---------------------------|-----------------|  
|Security|Activity by location|This report lists the countries from which activity originated in your cloud apps, and different parameters representing the volume of activity from each country, such as the number of events, number of users, etc. Use it to get an overview of the geographic distribution of your users.|  
|Security|Activity source by user|Users who performed activity in the cloud environment from several locations or using excessive amount of IP addresses. These users might be traveling, however it is possible that their credentials are misused.|  
|Security|Browser use|Browse- based attacks are among the most common attack vectors. Vendors invest enormous resources in securing browsing software, creating an effective update mechanism to disseminate updates to endpoints. Using deprecated browsers long after their update is due makes it an easy target for threat actors using available exploit kits. This report lists the browsers used in the last 30 days by users accessing your cloud services.|  
|Security|IP addresses|This report lists IP addresses used by devices to perform activities in your cloud environment protected by Cloud App Security. The report is based on audit logs accumulated by Cloud App Security. IP addresses are usually associated with a geographical location and with a source organization. Use this report to identify suspicious IP addresses connecting to your protected services. You may view the audit logs for each IP address by clicking on it.|  
|Security|IP addresses - privileged accounts|This report lists IP addresses used by devices to perform administrative activities in your cloud environment protected by Cloud App Security. The report is based on audit logs accumulated by Cloud App Security. IP addresses are usually associated with a geographical location and with a source organization. Use this report to identify suspicious IP addresses connecting to your protected services. You may view the audit logs for each IP address by clicking on it.|  
|Security|OS use|Operating system (OS) security flaws tend to cause very dangerous vulnerabilities. Vendors invest enormous resources in securing OSs, creating an effective update mechanism to disseminate updates to endpoints. However, deprecated OSs which are no longer supported, are not included in those update mechanisms, and they become easy targets for threat actors using available exploit kits. This report lists the OSs used in the last 30 days by users accessing your cloud services.|  
|Security|Strictly remote users|The following users have never shared an IP address with another employee in the company. This is characteristic to remote teams or employees, hired contractors and external support services. However, this may also indicate a backdoor user left by an attacker.|  
|User management|Cloud app overview|This report lists your cloud apps, and different parameters representing the volume of activity in each app, such as the number of files, users, etc. Use it to get an overview of the different apps and the extent to which your users use them.|  
|User management|Inactive accounts|Inactive accounts are accounts who have access to your cloud instance, yet they have not performed any events during the last 60 days. This suggests that these accounts are no longer active and should be suspended to prevent future access by threat actors or by leaving employees. Following this best-practice not only improves your security posture, but also reduces operational costs.|  
|User management|Privileged users|This report lists the users who have elevated privileges in corporate services, such as administrators. Privileged accounts such as these are a preferred attack vector for threat actors since they may allow them to gain substantial access to corporate information and network configuration. If there are privileged accounts that were not used in the past month, that might indicate a lack of IT security awareness in enterprises, potentially paving the way for a wave of data breaches. You may further investigate the use of elevated user privileges through the Audit Log, and consider revoking privileges when unnecessary.|  
|User management|Special privileged accounts|Salesforce has several types of privileged accounts, including Modify all data, View all data and Manage all users. Privileged accounts such as these are a preferred attack vector for threat actors since they may allow them to gain substantial access to corporate information and configurations.|  
|User management|User logon|This report details the number of log on attempts, number of successful log ons, and percentage of failed log on attempts made by each user in each service. A high percentage of failed log on attempts might indicate that a user account was under attack at some point.|  
|Data management|Data retention|Data retention policies deal with the issues of maintaining information in your possession for a pre-determined length of time, the procedures for archiving information, guidelines for destroying information when the time limit has been exceeded and special mechanisms for handling the information when under litigation. Data retention is a complicated balancing act. On one hand, you need to save information required by law and vital to your business. On the other hand, you should delete irrelevant, outdated and nonproductive data as quickly as possible. Use of the cloud for data storage increased complexity for the issue. Cloud data, just like hard copy data from years past, still needs to be retained for certain time periods based on legal, business, and personal requirements. Another benefit of enforcing data retention policies in your cloud environment is the ability to free storage space, reducing cloud operational costs. The following report provides you with visibility into data stored in your cloud environment which is a crucial step toward extending existing data retention policies to your cloud environment.|  
|Data management|Data sharing overview|This report lists the number of files stored in your cloud services, divided according to access permissions. Sharing has been made very easy with cloud services because of the ease of access and ubiquity.<br /><br /> A file that is not shared with anyone except its owner is referred to as a private file. If the file is shared, Cloud App Security differentiates between four types of states:<br /><br /> A publicly shared (web) file is a file that can be accessed without any authentication, even through a search engine result.<br /><br /> A publicly shared file is a file that can be accessed without any authentication, using a link.<br /><br /> An externally shared file is a file that can be accessed by individuals outside the organization, after authenticating themselves to the cloud service.<br /><br /> An internally shared file is a file that can be accessed by all or by some of your organization's users.|  
|Data management|File extensions|This report lists the extensions of files stored in your cloud services. Use it to get an overview of the file types in your cloud and how they are shared.|  
|Data management|Inbound sharing by domain|This report lists the domains from which files are shared with your employees. For each domain the report details which collaborators are sharing files, how many files are shared, and with whom the corporate users' files are shared. Accepting external collaboration is passive, therefore there is no policy to enforce on your employees. However, you might find that files which are supposed to be corporate files and are in fact externally owned and accessed via sharing, and in the worst case, phishing attacks can be launched against your employees through shared files.|  
|Data management|Orphan files|This report lists users who are suspended but still own files in one of your cloud services protected by Cloud App Security. These files are unmanaged and unaccounted for in case they violate compliance or policy. They should be either deleted or have their ownership transferred to an active user.|  
|Data management|Outbound sharing by domain|This report lists the domains with which corporate files are shared by your employees. For each domain the report details which corporate users are sharing files with that domain, which files are shared, and who are the collaborators files are shared with. It is advised that you manage the sharing with these domains via the Files tab in the service page of each relevant service.|  
|Data management|Owners of shared files|This report lists users who are sharing corporate files with the outside world. Externally shared files are shared with specific external collaborators. Publicly shared files are accessible to anyone on the internet, via a private link, and can be found only by those who are explicitly exposed to the link. Publicly shared files (Internet) are accessible to anyone on the internet even through a search engine result.  If you find users that share an excessive amount of files, it is advised that you investigate the nature of these excessive sharing permissions using the Files tab and contact these users to further understand their usage of external sharing.|  
|Data management|Personal user accounts|This report lists external user accounts with access to files in your cloud services protected by Cloud App Security, which are suspected as personal user accounts. The alleged owner of each personal account is noted in the column Corporate user. The pairing is calculated using our proprietary algorithm. Sharing corporate data with employees' personal accounts poses a threat to your sensitive materials as follows:<br /><br /> (1) Personal accounts are not provisioned by your security and IT teams. They may be compromised without their knowledge and they are not subject to the company's security policy (for example, password reset).<br /><br /> (2) Users may share corporate data on their personal accounts with less caution than they would with external collaborators.<br /><br /> (3) Internal collaborators may be subject to social engineering attacks. An attacker may use an account with a name that is similar to that of one of the employees (for example, john.doe@contoso.com or jdoe12@gmail.com) and gain access by requesting permission to sensitive data. Internal collaborators may unknowingly share corporate data with the attacker's account. The use of personal accounts is discouraged by Cloud App Security.|  
|Data management|Sensitive filenames|This report lists files which require your attention since their sharing permission might not suite their content, based on a heuristic scan of file names. This heuristic scan is helpful with identifying sensitive files without the need for a thorough content scan. Each file in the report is regarded as sensitive since according to the scan, it was identified as belonging to the categories detailed in the "Categories" column.|  
  
## See Also  
[Control](control.md)   
[For technical support, please visit the Cloud App Security assisted support page.](http://support.microsoft.com/oas/default.aspx?prid=16031)   
[Premier customers can also choose Cloud App Security directly from the Premier Portal.](https://premier.microsoft.com/)  
  
  