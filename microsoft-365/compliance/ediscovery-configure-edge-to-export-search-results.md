---
title: "Use the eDiscovery Export Tool in Microsoft Edge"
description: "You have to enable ClickOnce support to use the newest version of Microsoft Edge to download search results from Content Search and eDiscovery in the security and compliance portal."
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
ms.date: 01/01/2023
audience: Admin
ms.topic: how-to
ms.service: O365-seccomp
ms.collection:
- tier1
- purview-compliance
- ediscovery
search.appverid: 
- MOE150
- MET150
---

# Use the eDiscovery Export Tool in Microsoft Edge

As a result of recent changes to the newest version of Microsoft Edge, ClickOnce support is no longer enabled by default. To continue using the eDiscovery Export Tool to download Content Search or eDiscovery search results, you either need to use [Microsoft Internet Explorer](https://support.microsoft.com/help/17621/internet-explorer-downloads) or enable ClickOnce support in the newest version of Microsoft Edge.

[!INCLUDE [purview-preview](../includes/purview-preview.md)]

## Enable ClickOnce support in Microsoft Edge

1. In Microsoft Edge, go to **edge://flags/#edge-click-once**.
2. If the existing value is set to **Default** or **Disabled** in the dropdown list, change it to **Enabled**.

    ![Select Enabled from dropdown list.](../media/ClickOnceimage1.png)

3. Scroll down to the bottom of the browser window and select **Restart** to restart Microsoft Edge.

    ![Select Restart.](../media/ClickOnceimage2.png)

> [!NOTE]
> Organizations can use Group Policy to disable ClickOnce support. To check if there's an organizational policy for ClickOnce support, go to **edge://policy**. The following screenshot shows that ClickOnce is enabled across the entire organization. If this policy value is set to **false**, you'll need to contact an admin in your organization.

![List of Edge organizational policies.](../media/ClickOnceimage3.png)

## Install and run the eDiscovery Export Tool

1. Select **Download results** on the flyout page of an export in Content Search or an eDiscovery case.

    ![Select Download results on the flyout page to download search results.](../media/ClickOnceExport1.png)

1. You'll be prompted with a confirmation to launch the tool, select **Open**. If the eDiscovery Export Tool isn't installed, you'll be prompted with a Security Warning.

    ![Select Open to launch the eDiscovery Export Tool.](../media/ClickOnceimage4.png)

1. Select **Install**. After it's installed, the export tool will launch automatically.

For more information, see the following articles:

- [Export Content Search results](export-search-results.md)
- [How to enable experiment flags in Microsoft Edge](https://microsoftedgesupport.microsoft.com/hc/articles/360034075294-How-to-enable-experiment-flags-in-Microsoft-Edge-Insider-channels)
