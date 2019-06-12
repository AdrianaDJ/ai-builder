---
title: Use form processor component in PowerApps -  AI Builder | Microsoft Docs
description: Provides information about how to use the form processor component in PowerApps
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 06/07/2019
ms.author: v-dehaas
ms.reviewer: kvivek
---

# Use the form processor component in PowerApps

[!INCLUDE[cc-beta-prerelease-disclaimer](./includes/cc-beta-prerelease-disclaimer.md)]

Create a canvas app and add the form processor AI Builder component to your screen. This component takes a photo or loads an image from the local device, and then processes it to extract text based on a trained AI model. If it detects a form that the AI model is trained for, the form processor extracts the field values, and identifies them with rectangles.

 > [!NOTE] 
 > - Display of PDF files is not included in the initial preview.
 > - This component is not supported in Internet Explorer.
 > - Find more information about canvas apps [here](/powerapps/maker/canvas-apps/getting-started).

## Prerequisites
This component requires a trained and published AI Builder form processing model. Then, that model must be bound to the component using the AI model property in the properties panel.

When you add it to the screen, the component automatically opens the AI models pane to select a model from those published in that environment. 

The component is initialized after an AI model is bound to it.


<!--from editor: 
Because there's no text following the "Properties" heading, you could just delete it and promote "Key properties" and "Additional properties" to level 2. 
The "FormContent" bullet below ends with a colon, as if something is missing. 
-->


## Properties
### Key properties
 - **ModelId** (“AI model” in the properties panel): AI model information to which the component is bound.
 - **OriginalImage**: The original image before processing.
 - **FormContent**: The details of extracted form fields and tables. At component initialization (AI model binding step), the potential fields and tables that can be extracted by the models are populated:
 - **Fields**:

    ![Form fields screen](media/form-fields.PNG "Form fields screen")
    
 - **Tables**:

    ![Form tables screen](media/form-tables.PNG "Form tables screen") 

### Additional properties
 - **Text**: Text that appears on the button that activates the form processor.
 - **ImageDisplayed** (“Show image” in the properties panel): Whether the component displays the image or not. When set to ON, rectangles are displayed around field values detected in the image.


<!--from editor: What if, say, it's 40 percent. Is it red or orange? -->


- Three different colors can be used to draw the rectangle depending on the confidence level:
     - **Red**: Confidence level is between 0 percent and 40 percent.
     - **Orange**: Confidence level is between 40 percent and 70 percent.
     - **Blue**: Confidence level is between 70 percent and 100 percent.
 - **ShowConfidence** (“Show confidence” in the properties panel): Whether the component displays confidence levels along with the rectangles in the image or not.
 - **DisplayMode**:
     - **Edit**: Allows user input.
     - **View**: Only displays data. 
     - **Disabled** is disabled.
 - **Height**: The height of the component.
 - **Visible**: Whether the component appears or is hidden.
 - **Width**: The width of the component.
 - **X**: The distance between the left edge of the component and the left edge of its parent container (screen if no parent container).
 - **Y**: The distance between the top edge of the component and the top edge of the parent container (screen if no parent container).

Additional design properties are available in the Advanced panel.



<!--from editor: I get a 404 page with the Guidelines link and Core properties link. -->


## Accessibility guidelines
These [guidelines](/powerapps/maker/canvas-apps/controls/control-button) for the PowerApps button control also apply to the form processor component.

### Related topics

[Object detection model overview](object-detection-overview.md)<br/>
[Core properties in PowerApps](/powerapps/maker/canvas-apps/controls/properties-core)
