﻿---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
---
# UploadSession resource

Provides information about a [large file upload](../api/driveitem_createuploadsession.md) session.

## JSON representation

<!-- { "blockType": "resource", "@odata.type": "oneDrive.uploadSession" } -->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## Properties

| Property name          | Value                               | Description                                                                                  |
|:-----------------------|:------------------------------------|:---------------------------------------------------------------------------------------------|
| **uploadUrl**          | string                              | URL where fragment PUT requests should be directed.                                          |
| **expirationDateTime** | [timestamp](../resources/timestamp.md) | Date and time when the upload session expires.                                               |
| **nextExpectedRanges** | string array                        | An array of byte ranges the server is missing. Not always a full list of the missing ranges. |


<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->