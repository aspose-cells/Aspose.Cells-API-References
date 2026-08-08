---
title: "Workbook.save"
linktitle: "save"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Saves the workbook to the disk."
type: docs
weight: 790
url: /nodejs/aspose.cells/workbook/save/
---

## save(fileName, saveFormat)

Saves the workbook to the disk.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveFormat | Number | SaveFormat |

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var sheets = workbook.getWorksheets();
var cells = sheets.get(0).getCells();
cells.get("A1").putValue("Hello world!");
workbook.save("Book1.xls", aspose.cells.SaveFormat.EXCEL_97_TO_2003);
```
