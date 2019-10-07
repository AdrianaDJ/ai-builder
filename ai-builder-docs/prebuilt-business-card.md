---
title: Overview of prebuilt AI models -  AI Builder | Microsoft Docs
description: Describes the prebuilt AI models that are available in AI Builder.
author: alanabrito
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 10/04/2019
ms.author: alanab
ms.reviewer: v-dehaas
---

# Prebuilt business card AI model

The prebuilt business card AI model allows you to extract contact information from business cards images. If the business card is detected in the image, information such as name, job title, address, email, company and phone numbers can be extracted.


## Use in PowerApps

If you want to use this prebuilt model in PowerApps using the Business card reader component. You can find more information in [Use business card reader component in PowerApps](business-card-reader-component-in-powerapps.md).

## Use in Microsoft Flow

If you want to use this prebuilt model in Microsoft Flow, you can find more information in Use business card model in Microsoft Flow.
 
## Supported language, format and size

The images you can process with the business card model need these characteristics:

- Language: English.  
- Format: 
    - JPG 
    - PNG 
    - BMP 
- Size: 6 MB maximum 
 
## Model output 
If a business card is detected, the business card model will try to locate and extract the following properties:

|Property |Definition  |
|---------|---------|
| **AddressCity**| The city address|
| **AddressCountry**| The country address|
| **AddressPostalCode**| The postal code address|
| **AddressStreet**| The street address|
| **BusinessPhone**| The first phone or fax number|
| **CleanedImage**| The image after processing where the business card appears cropped and enhanced from the original image|
| **CompanyName**| The company name|
| **Department**| The organization department found|
| **Email**| The contact email found in the business card, if any|
| **Fax**| The third phone or fax number|
| **FirstName**| The contact first name|
| **FullAddress**| The contact full address|
| **FullName**| The contact full name|
| **JobTitle**| The contact job title|
| **LastName**| The contact last name|
| **MobilePhone**| The second phone or fax number|
| **OriginalImage**| The original image before processing|
| **Website**| The website|
