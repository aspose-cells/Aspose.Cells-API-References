---
title: "Sparkline.toImageStream"
linktitle: "toImageStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Converts a sparkline to an image."
type: docs
weight: 70
url: /nodejs/aspose.cells/sparkline/toimagestream/
---

## toImageStream(sparkline, stream, options) (static)

Converts a sparkline to an image.

| Parameter | Type | Description |
| --- | --- | --- |
| sparkline | Sparkline | The Sparkline object |
| stream | WritableStream | The stream of the output image |
| options | ImageOrPrintOptions | Addtional image creation options |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("sparkline.xlsx");
var sparkline = workbook.getWorksheets().get(0).getSparklineGroupCollection().get(0).getSparklineCollection().get(0);
var imgWriteStream = fs.createWriteStream("sparkline.jpeg");
var imgOptions = new aspose.cells.ImageOrPrintOptions();
imgOptions.setHorizontalResolution(200);
imgOptions.setVerticalResolution(300);
imgOptions.setImageFormat(aspose.cells.ImageFormat.getJpeg());
aspose.cells.Sparkline.toImageStream(sparkline, imgWriteStream, imgOptions);
```
