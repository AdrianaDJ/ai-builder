---
title: Create a prediction model -  AI Builder | Microsoft Docs
description: This topic lays out the steps you need to follow to create a prediction model in AI Builder. 
author: Dean-Haas
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 06/07/2019
ms.author: sdarapu
ms.reviewer: kvivek
---

# Create a prediction model

This example creates a PowerApps prediction AI model that uses the *online shopper intention* Common Data Service entity.  To get this sample data into your Common Data Service environment. enable the **Deploy sample apps and data** setting when you create an environment as described [here](build-model.md). Or, follow the more detailed instructions [here](binary-classification-data-prep.md). After your sample data is in Common Data Service, follow these steps to create your model:

1. Sign in to [PowerApps](https://web.powerapps.com) and then select **AI Builder (preview)** > **Build**. 
2. Select **prediction**. Enter a model name and then select **Create**.
3. Select **Online shopper intention** as the entity, and **Label** as the field.

## Select the data fields to train your model

After you select the **Entity** and **Label** fields and map your outcome, the next step is to find related entities to help predict the outcome. By default, fields for your target entity and all related entities and fields are selected. You could deselect data fields that might not be important for your business or which might carry unwanted bias. 
 
 ### Data field selection considerations
- Make sure you select the data fields that you want to use in training the model. 
- Deselect the data fields that do not address the problem you want to solve. 
- Deselect the data fields that might carry unwanted bias.
- Make sure the data fields you select don't have a high rate of missing values. If it is a valuable data field, you can assign a default value.
 
> [!NOTE]
> These Common Data Service data types are excluded from the prediction model. These will not appear in the **Field** drop-down menu: 
> - Customer
> - Image
> - Lookup
> - Multiple selection Option set
> - Multiline Text
> - Owner
> - Unique Identifier
> - String type data types with length greater than 100 characters 

### Next step
[Train and publish your prediction model](binary-classification-train-model.md)<br/>
