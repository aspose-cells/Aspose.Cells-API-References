---
title: "Worksheet.protect"
linktitle: "protect"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Protects worksheet."
type: docs
weight: 1060
url: /nodejs/aspose.cells/worksheet/protect-1/
---

## protect(type, password, oldPassword)

Protects worksheet. This method can protect worksheet in all versions of Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ProtectionType |
| password | String | Password. |
| oldPassword | String | If the worksheet is already protected by a password, please supply the old password. Otherwise, you can set a null value or blank string to this parameter. |

**Example:**

```js
//Instantiating a Workbook object
var excel = new aspose.cells.Workbook("Book2.xls");
//Accessing the first worksheet in the Excel file
var worksheet = excel.getWorksheets().get(0);
//Protecting the worksheet with a password
worksheet.protect(aspose.cells.ProtectionType.ALL, "aspose", null);
//Saving the modified Excel file in default (that is Excel 20003) format
excel.save("Book1.xls");
```
