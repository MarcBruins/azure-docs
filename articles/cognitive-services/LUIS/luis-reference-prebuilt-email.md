---
title: LUIS Prebuilt entities email reference - Azure| Microsoft Docs
titleSuffix: Azure
description: This article contains email prebuilt entity information in Language Understanding (LUIS).
services: cognitive-services
author: diberry
manager: cgronlun
ms.custom: seodec18
ms.service: cognitive-services
ms.component: language-understanding
ms.topic: article
ms.date: 11/27/2018
ms.author: diberry
---

# Email prebuilt entity for a LUIS app
Email extraction includes the entire email address from an utterance. Because this entity is already trained, you do not need to add example utterances containing email to the application intents. Email entity is supported in `en-us` culture only. 

## Resolution for prebuilt email
The following example shows the resolution of the **builtin.email** entity.

```json
{
  "query": "please send the information to patti.owens@microsoft.com",
  "topScoringIntent": {
    "intent": "None",
    "score": 0.811592042
  },
  "intents": [
    {
      "intent": "None",
      "score": 0.811592042
    }
  ],
  "entities": [
    {
      "entity": "patti.owens@microsoft.com",
      "type": "builtin.email",
      "startIndex": 31,
      "endIndex": 55
    }
  ]
}
```

## Next steps

Learn about the [number](luis-reference-prebuilt-number.md), [ordinal](luis-reference-prebuilt-ordinal.md), and [percentage](luis-reference-prebuilt-percentage.md). 