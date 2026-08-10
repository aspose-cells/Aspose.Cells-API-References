---
title: "ReConnectionMethodType"
linktitle: "ReConnectionMethodType"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Utility class containing constants."
type: docs
weight: 2150
url: /nodejs/global/reconnectionmethodtype/
---

## ReConnectionMethodType

Utility class containing constants. Specifies what the spreadsheet application should do when a connection fails.

## Values

| Name | Description |
| --- | --- |
| REQUIRED | On refresh use the existing connection information and if it ends up being invalid then get updated connection information, if available from the external connection file. |
| ALWAYS | On every refresh get updated connection information from the external connection file, if available, and use that instead of the existing connection information. In this case the data refresh will fail if the external connection file is unavailable. |
| NEVER | Never get updated connection information from the external connection file even if it is available and even if the existing connection information is invalid |
