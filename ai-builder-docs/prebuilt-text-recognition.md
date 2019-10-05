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

# Text recognition model

The prebuild text recognition model can be used to extract recognized words from documents and images into machine-readable character streams. It uses state-of-the-art optical character recognition (OCR) to detect embedded printed and handwritten text.

This prebuilt processes images and document files to extract lines of printed or handwritten text.


## Use in PowerApps

If you want to use this prebuilt model in Microsoft Flow, you can find more information in Use text recognition model in Microsoft Flow.  

## Supported language, format and size 

The documents you can scan with the Text recognition model need these characteristics:

- **Language**: English
- **Format**:
    - JPG
    - PNG
    - BMP
    - PDF
    - TIFF
- **Size**: 20 MB maximum
 
## Model output

If a document is detected, the text recognition model will output the following information:

- **Results**: A list of lines extracted from the input text.
- **Text**: Strings containing the line of text detected.
- **BoundingBox**: Four values representing the bounding box, described using the top and left positions along with its width and height. 
