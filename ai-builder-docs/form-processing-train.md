---
title: Test your form processing model -  AI Builder | Microsoft Docs
description: Walks you through the steps to train, validate, and test your form processing model in AI Builder.
author: Dean-Haas
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 06/07/2019
ms.author: v-dehaas
ms.reviewer: kvivek
---

# Test your form processing model

[!INCLUDE[cc-beta-prerelease-disclaimer](./includes/cc-beta-prerelease-disclaimer.md)]

After you create your form processing model, you can train, test, and publish it to make it available.

## Train and validate your model

1. Select **Next** to check your selected form fields. If everything looks good, select **Train** to train your model. 
1. When training completes,  select **Go to Details page** in the **Training complete** screen.

## Quick-test your model 

The Details page allows you to test your model before you publish or use it:

1. On the Details page, select **Quick test**.
2. You can either drag and drop a document, or select **Upload from my device** to upload your test file. The quick-test should only take a few seconds before displaying the results. 
3. You can select **Start over** to run another test or **Close** if you are finished.

## Troubleshooting tips

If you have trouble training your model, try the following:

- Optimize your data using the guidance in the [Requirements](form-processing-model-requirements.md) topic. 
- Delete and recreate the model. 
- Download and test with [sample material](http://aka.ms/AIBuilderMBASLab). 

## Publish your model

If you’re happy with your model, you can select **Publish**  to publish it. When publishing completes, your model is promoted as **Published** and is ready to be used. For more information about publishing your model, go to [Publish your model](publish-model.md) section.

After you’ve published your form processing model, you can use it in a canvas app or in Microsoft Flow.

### Related topics
[Form processing model in Flow](form-processing-model-in-flow.md) </br>
[Form processing model in PowerApps](form-processor-component-in-powerapps.md)
