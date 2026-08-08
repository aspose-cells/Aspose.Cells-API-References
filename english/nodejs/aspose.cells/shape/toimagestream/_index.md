---
title: "Shape.toImageStream"
linktitle: "toImageStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Saves the shape to a stream."
type: docs
weight: 1950
url: /nodejs/aspose.cells/shape/toimagestream/
---

## toImageStream(shape, stream, options) (static)

Saves the shape to a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| shape | Shape | The Shape object |
| stream | WritableStream | The stream of the output image |
| options | ImageOrPrintOptions | Addtional image creation options |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var shape = workbook.getWorksheets().get("Shape").getShapes().get(0);
var imgWriteStream = fs.createWriteStream("shape1.jpeg");
var imgOptions = new aspose.cells.ImageOrPrintOptions();
imgOptions.setHorizontalResolution(200);
imgOptions.setVerticalResolution(300);
imgOptions.setImageFormat(aspose.cells.ImageFormat.getJpeg());
aspose.cells.Shape.toImageStream(shape, imgWriteStream, imgOptions);
```
