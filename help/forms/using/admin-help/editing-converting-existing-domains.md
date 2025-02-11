---
title: Editing and converting existing domains
seo-title: Editing and converting existing domains
description: Learn how to change the settings for existing domains from the Domain Management page. Convert an existing enterprise domain to a hybrid domain or vice versa. 
seo-description: Learn how to change the settings for existing domains from the Domain Management page. Convert an existing enterprise domain to a hybrid domain or vice versa. 
uuid: 4cc9547e-b4ec-4588-b1cf-18720f06149a
contentOwner: admin
content-type: reference
geptopics: SG_AEMFORMS/categories/setting_up_and_managing_domains
products: SG_EXPERIENCEMANAGER/6.4/FORMS
discoiquuid: 44dec184-3ef7-4ba6-a87f-ad171d3cb188
exl-id: 07ca7715-f7b3-40e0-95bc-e05f0662ed08
---
# Editing and converting existing domains{#editing-and-converting-existing-domains}

You can change the settings for existing domains from the Domain Management page. You can also convert an existing enterprise domain to a hybrid domain.

## Edit an existing domain {#edit-an-existing-domain}

1. In administration console, click Settings &gt; User Management &gt; Domain Management.
1. Click the name of the domain to edit. 
1. To change the domain name, change the text in the Name box. 
1. To change the authentication information for an enterprise or hybrid domain, click the appropriate authentication name at the bottom of the page. On the Edit Authentication page, change settings as required. (See [Authentication settings](/help/forms/using/admin-help/configuring-authentication-providers.md#authentication-settings).)
1. To change the directory information for an enterprise domain, click the appropriate directory name at the bottom of the page. On the Edit Directory page, change settings as required. (See [Adding directories or custom SPIs](/help/forms/using/admin-help/configuring-directories.md#adding-directories-or-custom-spis).)
1. When you complete your changes, click OK.

## Convert an enterprise domain to a hybrid domain {#convert-an-enterprise-domain-to-a-hybrid-domain}

1. In administration console, click Settings &gt; User Management &gt; Domain Management.
1. Click the name of the enterprise domain to convert. 
1. Click Convert to Hybrid Domain.
1. Review the information that appears regarding user and group data and authentication of users, and click OK.
1. Edit the settings for the hybrid domain and click OK.

>[!NOTE]
>
>If the enterprise domain that you are converting does not contain directory settings, any LDAP authentication settings are lost.

## Convert a hybrid domain to an enterprise domain {#convert-a-hybrid-domain-to-an-enterprise-domain}

1. In administration console, click Settings &gt; User Management &gt; Domain Management.
1. Click the name of the hybrid domain to convert. 
1. Click Convert to Enterprise Domain.
1. Review the information that appears regarding user and group data and authentication of users, and click OK.
1. Click Add Directory and configure the required directory information. (See [Adding directories or custom SPIs](/help/forms/using/admin-help/configuring-directories.md#adding-directories-or-custom-spis).)
