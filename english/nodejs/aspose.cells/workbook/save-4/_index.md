---
title: "Workbook.save"
linktitle: "save"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Save the workbook to the stream."
type: docs
weight: 990
url: /nodejs/aspose.cells/workbook/save-4/
---

## save(workbook, stream, saveFormat) (static)

Save the workbook to the stream.

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook object to save |
| stream | WritableStream | The stream |
| saveFormat | Number | The save file format type |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var writeStream = fs.createWriteStream("result-stream.xlsx");
aspose.cells.Workbook.saveToStream(workbook, writeStream, aspose.cells.SaveFormat.XLSX);
```
