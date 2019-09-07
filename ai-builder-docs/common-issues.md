---
title:  Common issues and resolutions for AI Builder -  AI Builder | Microsoft Docs
description: Provides a list of common issues you might encounter while using AI Builder, and potential workarounds where applicable.
author: Dean-Haas
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 08/27/2019
ms.author: joshrenn
ms.reviewer: kvivek
---

# Common issues and resolutions for AI Builder 

Here are some issues that you might encounter when you  use AI Builder. Where applicable, workarounds are provided.

### AI Builder is not set up correctly in your environment

If you are using an environment that was created before AI Builder was first released, it is possible that AI Builder may have not been set up correctly in your environment. To work around this issue, [create a new environment](https://docs.microsoft.com/power-platform/admin/create-environment) so that AI Builder can be correctly installed in that new environment. If you must use a particular environment, [contact support](https://docs.microsoft.com/power-platform/admin/get-help-support) for more options.

### AI Builder encounters errors reading data from your Common Data Service entity

Use the navigation links on the left side of your screen to locate the data preparation section for the type of AI model that you are working with. Make sure your Common Data Service instance is configured correctly so that your model can access it.

### AI Builder business card reader doesn't work for some users

Make sure that the user of the business card reader component has permissions in Common Data Service, or has access to the AI Builder model entity that is configured in the business card reader component.

## Ask the community

You can also check Microsoft community forums to see if other users have posted a solution that might help you. 

- [AI Builder community]((https://go.microsoft.com/fwlink/?linkid=2092048))
- [Common Data Service community forums](https://powerusers.microsoft.com/t5/Common-Data-Services/ct-p/PA_CommonDataServices)
- [PowerApps community forums](https://powerusers.microsoft.com/t5/Forums/ct-p/PA_Comm_Forums)
