---
title: "WorkbookRender Class"
linktitle: "WorkbookRender"
articleTitle: "WorkbookRender"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a Workbook render."
type: docs
weight: 7580
url: /php/aspose.cells/workbookrender/
---

## WorkbookRender class

Represents a Workbook render. The constructor of this class , must be used after modification of pagesetup, cell style.

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookRender](#constructor) | The construct of WorkbookRender |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [PageCount](#pagecount) | Number | Gets the total page count of workbook. |

## Methods

| Name | Description |
| --- | --- |
| [getPageSizeInch](#getpagesizeinch) | Get page size in inch of output image. |
| [toImage](#toimage) | Render whole workbook as Tiff Image to a file. |
| [toPrinter](#toprinter) | Render workbook to Printer |

### WorkbookRender(workbook, options) {#constructor}

The construct of WorkbookRender

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | Indicate which workbook to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |

### WorkbookRender.PageCount property {#pagecount}

Gets the total page count of workbook.

**Type:** Number

### getPageSizeInch(pageIndex) {#getpagesizeinch}

Get page size in inch of output image.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | The page index is based on zero. |

**Returns:** Page size of image, [0] for width and [1] for height

### toImage(filename) (1 of 3) {#toimage}

Render whole workbook as Tiff Image to a file.

| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | the filename of the output image |

---

### toImage(pageIndex, fileName) (2 of 3) {#toimage-1}

Render certain page to a file.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | indicate which page is to be converted |
| fileName | String | filename of the output image |

---

### toImage(pageIndex, stream) (3 of 3) {#toimage-2}

Render certain page to a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | indicate which page is to be converted |
| stream | OutputStream | the stream of the output image |

### toPrinter(printerName) (1 of 2) {#toprinter}

Render workbook to Printer

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |

---

### toPrinter(printerName, jobName) (2 of 2) {#toprinter-1}

Render workbook to Printer

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| jobName | String | set the print job name |
