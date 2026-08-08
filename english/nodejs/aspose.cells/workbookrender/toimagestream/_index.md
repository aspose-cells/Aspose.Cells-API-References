---
title: "WorkbookRender.toImageStream"
linktitle: "toImageStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Render whole workbook as Tiff Image to stream."
type: docs
weight: 90
url: /nodejs/aspose.cells/workbookrender/toimagestream/
---

## toImageStream(workbookRender, stream) (static)

Render whole workbook as Tiff Image to stream.

| Parameter | Type | Description |
| --- | --- | --- |
| workbookRender | WorkbookRender | The WorkbookRender object |
| stream | WritableStream | The stream of the output image |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var imgOptions = new aspose.cells.ImageOrPrintOptions();
imgOptions.setHorizontalResolution(200);
imgOptions.setVerticalResolution(300);
imgOptions.setSaveFormat(aspose.cells.SaveFormat.XPS);
var workbookRender = new aspose.cells.WorkbookRender(workbook, imgOptions);
var imgWriteStream = fs.createWriteStream("workbook.xps");
aspose.cells.WorkbookRender.toImageStream(workbookRender, imgWriteStream);
```
