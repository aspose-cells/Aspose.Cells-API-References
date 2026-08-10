---
title: "SheetRender"
linktitle: "SheetRender"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after m"
type: docs
weight: 3680
url: /nodejs/aspose.cells/sheetrender/
---

## SheetRender class

Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after modification of pagesetup, cell style.

```js
new SheetRender(worksheet, options)
```

the construct of SheetRender, need worksheet and ImageOrPrintOptions as params

## Methods

| Name | Description |
| --- | --- |
| [getPageCount()](#getpagecount) | Gets the total page count of current worksheet. |
| [getPageScale()](#getpagescale) | Gets calculated page scale of the sheet. Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculat |
| [getPageSizeInch(pageIndex)](#getpagesizeinch) | Get page size in inch of output image. |
| [toImage(pageIndex, fileName)](#toimage) | Render certain page to a file. |
| [toPrinter(printerName)](#toprinter) | Render worksheet to Printer |
| [toPrinter(printerName, jobName)](#toprinter-1) | Render worksheet to Printer |
| [toImageStream(sheetRender, pageIndex, stream)](#toimagestream) *(static)* | Render certain page to a stream. |

### getPageCount() {#getpagecount}

Gets the total page count of current worksheet.

### getPageScale() {#getpagescale}

Gets calculated page scale of the sheet. Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculated scale according to PageSetup.FitToPagesWide and PageSetup.FitToPagesTall.

### getPageSizeInch(pageIndex) {#getpagesizeinch}

Get page size in inch of output image.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | The page index is based on zero. |

**Returns:** Array of float — `Array of float` Page size of image, [0] for width and [1] for height

### toImage(pageIndex, fileName) {#toimage}

Render certain page to a file.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | indicate which page is to be converted |
| fileName | String | filename of the output image |

### toPrinter(printerName) {#toprinter}

Render worksheet to Printer

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |

### toPrinter(printerName, jobName) {#toprinter-1}

Render worksheet to Printer

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| jobName | String | set the print job name |

### toImageStream(sheetRender, pageIndex, stream) (static) {#toimagestream}

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
