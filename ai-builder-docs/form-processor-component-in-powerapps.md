---
title: Use form processor component in Power Apps -  AI Builder | Microsoft Docs
description: Provides information about how to use the form processor component in Power Apps
author: JoeFernandezMS
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 12/31/2019
ms.author: jofernan
ms.reviewer: v-dehaas
---

# Use the form processor component in Power Apps

You can add the AI Builder form processor component to your screen in your canvas apps. This component takes a photo or loads your image. Then, it extracts text based on your trained AI model. If it detects a form that the AI model is trained for, the form processor extracts the field values, and identifies them with rectangles.

 > [!NOTE]
 >
 > - Display of PDF files is not included in the initial preview.
 > - For more information about canvas apps, see [What are canvas apps in PowerApps?](/powerapps/maker/canvas-apps/getting-started).

## Prerequisites

This component requires a published AI Builder form processing model. Then, that model must be bound to the component using the AI model property in the properties panel.

When you add the component to the screen, it automatically opens the AI models pane. There, you select a model that is published in your environment.

The component is initialized after an AI model is bound to it.


## Key properties

 - **ModelId** ("AI model" in the properties panel): AI model information to which the component is bound.
 - **OriginalImage**: The original image before processing.
 - **FormContent**: The details of extracted form fields and tables. At component initialization (AI model binding step), the fields and tables that can be extracted by the models are populated:
   - **Fields**:

     ![Form fields screen](media/form-fields.png "Form fields screen")

   - **Tables**:

     ![Form tables screen](media/form-tables.png "Form tables screen")

## Additional properties

- **Text**: Text that appears on the button that activates the form processor.
- **ImageDisplayed** ("Show image" in the properties panel): Whether or not the component displays the image. When set to ON, rectangles are displayed around field values detected in the image.

- Three different colors can be used to draw the rectangle depending on the confidence level:
     - **Red**: Confidence level is between 0 percent and 39 percent.
     - **Orange**: Confidence level is between 40 percent and 59 percent.
     - **Blue**: Confidence level is between 60 percent and 100 percent.
- **ShowConfidence** ("Show confidence" in the properties panel): Whether the component displays confidence levels along with the rectangles in the image or not.
- **DisplayMode**:
     - **Edit**: Allows user input.
     - **View**: Only displays data.
     - **Disabled** is disabled.
- **Height**: The height of the component.
- **Visible**: Whether the component appears or is hidden.
- **Width**: The width of the component.
- **X**: The distance between the left edge of the component and the left edge of its parent container or screen.
- **Y**: The distance between the top edge of the component and the top edge of the parent container or screen.

Additional design properties are available in the Advanced panel.

## Accessibility guidelines
These [guidelines](/powerapps/maker/canvas-apps/controls/control-button) for the Power Apps button control also apply to the form processor component.

### Related topics

[Object detection model overview](object-detection-overview.md)

[Core properties in Power Apps](/powerapps/maker/canvas-apps/controls/properties-core)
