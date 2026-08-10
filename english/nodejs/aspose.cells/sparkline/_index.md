---
title: "Sparkline"
linktitle: "Sparkline"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data."
type: docs
weight: 3850
url: /nodejs/aspose.cells/sparkline/
---

## Sparkline class

A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.

## Methods

| Name | Description |
| --- | --- |
| [getColumn()](#getcolumn) | Gets the column index of the sparkline. |
| [getDataRange()](#getdatarange) | Represents the data range of the sparkline. |
| [getRow()](#getrow) | Gets the row index of the sparkline. |
| [setDataRange()](#setdatarange) | Represents the data range of the sparkline. |
| [toImage(fileName, options)](#toimage) | Converts a sparkline to an image. |
| [toImage(stream, options)](#toimage-1) | Converts a sparkline to an image. |
| [toImageStream(sparkline, stream, options)](#toimagestream) *(static)* | Converts a sparkline to an image. |

### getColumn() {#getcolumn}

Gets the column index of the sparkline.

### getDataRange() {#getdatarange}

Represents the data range of the sparkline.

### getRow() {#getrow}

Gets the row index of the sparkline.

### setDataRange() {#setdatarange}

Represents the data range of the sparkline.

### toImage(fileName, options) {#toimage}

Converts a sparkline to an image.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The image file name. |
| options | ImageOrPrintOptions | The image options |

### toImage(stream, options) {#toimage-1}

Converts a sparkline to an image.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | OutputStream | The image stream. |
| options | ImageOrPrintOptions | The image options. |

### toImageStream(sparkline, stream, options) (static) {#toimagestream}

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
