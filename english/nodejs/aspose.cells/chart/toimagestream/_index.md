---
title: "Chart.toImageStream"
linktitle: "toImageStream"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Creates the chart image and saves it to a stream in the specified format."
type: docs
weight: 1000
url: /nodejs/aspose.cells/chart/toimagestream/
---

## toImageStream(chart, stream, options) (static)

Creates the chart image and saves it to a stream in the specified format. The format of the image is specified by using options.ImageFormat. The following formats are supported: ImageFormat.Bmp, ImageFormat.Gif, ImageFormat.Png, ImageFormat.Jpeg, ImageFormat.Tiff, ImageFormat.Emf. If the width or height is zero or the chart is not supported according to Supported Charts List, this method will do nothing. Please refer to Supported Charts List for more details.

| Parameter | Type | Description |
| --- | --- | --- |
| chart | Chart | The Chart object |
| stream | WritableStream | The stream of the output image |
| options | ImageOrPrintOptions | Addtional image creation options |

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
imgWriteStream = fs.createWriteStream("chart.jpeg");
var chart = workbook.getWorksheets().get("Chart").getCharts().get(0);
aspose.cells.Chart.toImageStream(chart, imgWriteStream, imgOptions);
```
