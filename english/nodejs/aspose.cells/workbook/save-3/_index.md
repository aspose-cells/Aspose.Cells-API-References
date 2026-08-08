---
title: "Workbook.save"
linktitle: "save"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Save the workbook to the stream."
type: docs
weight: 980
url: /nodejs/aspose.cells/workbook/save-3/
---

## save(workbook, stream, saveOptions) (static)

Save the workbook to the stream.

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook object to save |
| stream | WritableStream | The stream |
| saveOptions | SaveOptions | The save options |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var saveOptions = new aspose.cells.XlsSaveOptions();
var writeStream = fs.createWriteStream("result-stream.xls");
aspose.cells.Workbook.saveToStream(workbook, writeStream, saveOptions);
```
