---
title: Create a form processing model | Microsoft Docs
description: Provides steps to create a form processing model in Builder.
author: Dean-Haas
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 06/10/2019
ms.author: v-dehaas
ms.reviewer: kvivek
---

# Create a form processing model

[!INCLUDE[cc-beta-prerelease-disclaimer](./includes/cc-beta-prerelease-disclaimer.md)]

When  you create your form processing model, you’ll need to do the following:
1. Run analysis on your sample form documents.
2. Select the form fields that you want the model to remember.
3. Review your model and train it.
4. Evaluate your model (optional)


## Upload and analyze documents
You need to provide sample documents to train your model for the type of form from which you want to extract information. After you upload your documents, AI Builder analyzes them so you can tell whether you can train a model from them.
### Upload your documents
1. Sign in to [PowerApps](https://web.powerapps.com), and then in the navigation pane, select **AI Builder (preview)** > **Build**. Then, select the Form processing AI model type.
2. Enter a name for your model then select **Create**. 
3. Select **Add documents**, select a minimum of 5 documents, and then select **Upload**.

For more information about requirements for input documents please see [Requirements and limitations](form-processing-model-requirements.md).
> [!NOTE] 
>
> After you upload these documents, you can still remove some of the documents or upload additional ones.

### Analyze your documents
When enough documents have been uploaded, you select **Analyze** to launch the analysis. Depending on the number of documents provided, the analysis could take longer but in most cases it should only take a few minutes.

## Review documents and extracted data
If the analysis was successful, it means we’ve detected structured text in your form documents. If the analysis failed, it is likely because AI Builder couldn't detect structured text in your documents.

 
## Select your form fields
To start, choose the fields that matter to you:
 1. Select the detected template card: **\<*Your project name*> template**.
 1. To select the fields, hover over a rectangle that indicates a detected field in the document, or select them in the right-side pane.
 1. Select the **Edit** button next to the selected field if you want to rename fields to align with your needs or normalize the extracted labels.

    When you hover over a detected field, the following information appears:
- **Field name**: The name of the label for the detected field.
- **Field value**: The value for the detected field.
- **Confidence level**: Confidence score of retrieving this field compared to the trained model.


### Next steps
[Train and publish your form processing model](form-processing-train.md)

### Related topics
[Form processing model in Flow](form-processing-model-in-flow.md)
[Form processing model in PowerApps](form-processor-component-in-powerapps.md)