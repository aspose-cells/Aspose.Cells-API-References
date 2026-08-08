---
title: "WorkbookRender"
linktitle: "WorkbookRender"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a Workbook render."
type: docs
weight: 4710
url: /nodejs/aspose.cells/workbookrender/
---

## WorkbookRender class

Represents a Workbook render. The constructor of this class , must be used after modification of pagesetup, cell style.

```js
new WorkbookRender(workbook, options)
```

The construct of WorkbookRender

## Methods

| Name | Description |
| --- | --- |
| [getPageCount()](#getpagecount) | Gets the total page count of workbook. |
| [getPageSizeInch(pageIndex)](#getpagesizeinch) | Get page size in inch of output image. |
| [toImage(filename)](#toimage) | Render whole workbook as Tiff Image to a file. |
| [toImage(pageIndex, fileName)](#toimage-1) | Render certain page to a file. |
| [toImage(pageIndex, stream)](#toimage-2) | Render certain page to a stream. |
| [toPrinter(printerName)](#toprinter) | Render workbook to Printer |
| [toPrinter(printerName, jobName)](#toprinter-1) | Render workbook to Printer |
| [toImageStream(workbookRender, stream)](#toimagestream) *(static)* | Render whole workbook as Tiff Image to stream. |

### getPageCount() {#getpagecount}

Gets the total page count of workbook.

### getPageSizeInch(pageIndex) {#getpagesizeinch}

Get page size in inch of output image.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | The page index is based on zero. |

**Returns:** Array of float — `Array of float` Page size of image, [0] for width and [1] for height

### toImage(filename) {#toimage}

Render whole workbook as Tiff Image to a file.

| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | the filename of the output image |

### toImage(pageIndex, fileName) {#toimage-1}

Render certain page to a file.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | indicate which page is to be converted |
| fileName | String | filename of the output image |

### toImage(pageIndex, stream) {#toimage-2}

Render certain page to a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | indicate which page is to be converted |
| stream | OutputStream | the stream of the output image |

### toPrinter(printerName) {#toprinter}

Render workbook to Printer

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |

### toPrinter(printerName, jobName) {#toprinter-1}

Render workbook to Printer

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| jobName | String | set the print job name |

### toImageStream(workbookRender, stream) (static) {#toimagestream}

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
