---
title: "Shape.toImageStream"
linktitle: "toImageStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Creates the shape image and saves it to a stream in the specified format."
type: docs
weight: 1960
url: /nodejs/aspose.cells/shape/toimagestream-1/
---

## toImageStream(shape, stream, imageFormat) (static)

Creates the shape image and saves it to a stream in the specified format. The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

| Parameter | Type | Description |
| --- | --- | --- |
| shape | Shape | The Shape object |
| stream | WritableStream | The stream of the output image |
| imageFormat | ImageFormat | The format in which to save the image |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var shape = workbook.getWorksheets().get("Shape").getShapes().get(0);
var imangeFormatJpeg = aspose.cells.ImageFormat.getJpeg();
imgWriteStream = fs.createWriteStream("shape2.jpeg");
shape = workbook.getWorksheets().get("Shape").getShapes().get(1);
aspose.cells.Shape.toImageStream(shape, imgWriteStream, imangeFormatJpeg);
```
