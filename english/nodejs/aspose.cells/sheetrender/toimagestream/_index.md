---
title: "SheetRender.toImageStream"
linktitle: "toImageStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Render certain page to a stream."
type: docs
weight: 80
url: /nodejs/aspose.cells/sheetrender/toimagestream/
---

## toImageStream(sheetRender, pageIndex, stream) (static)

Render certain page to a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetRender | SheetRender | The SheetRender object |
| pageIndex | Number | Indicate which page is to be converted |
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
imgOptions.setImageFormat(aspose.cells.ImageFormat.getJpeg());
var worksheet = workbook.getWorksheets().get(0);
var sheetRender = new aspose.cells.SheetRender(worksheet, imgOptions);
var imgWriteStream = fs.createWriteStream("sheet1.jpeg");
aspose.cells.SheetRender.toImageStream(sheetRender, 0, imgWriteStream);
```
