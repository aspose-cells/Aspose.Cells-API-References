---
title: "SheetRender Class"
linktitle: "SheetRender"
articleTitle: "SheetRender"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after m"
type: docs
weight: 5990
url: /php/aspose.cells/sheetrender/
---

## SheetRender class

Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after modification of pagesetup, cell style.

## Constructors

| Name | Description |
| --- | --- |
| [SheetRender](#constructor) | the construct of SheetRender, need worksheet and ImageOrPrintOptions as params |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [PageCount](#pagecount) | Number | Gets the total page count of current worksheet. |
| [PageScale](#pagescale) | Number | Gets calculated page scale of the sheet. Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculat |

## Methods

| Name | Description |
| --- | --- |
| [getPageSizeInch](#getpagesizeinch) | Get page size in inch of output image. |
| [toImage](#toimage) | Render certain page to a file. |
| [toPrinter](#toprinter) | Render worksheet to Printer |

### SheetRender(worksheet, options) {#constructor}

the construct of SheetRender, need worksheet and ImageOrPrintOptions as params

| Parameter | Type | Description |
| --- | --- | --- |
| worksheet | Worksheet | Indicate which spreadsheet to be rendered. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |

### SheetRender.PageCount property {#pagecount}

Gets the total page count of current worksheet.

**Type:** Number

### SheetRender.PageScale property {#pagescale}

Gets calculated page scale of the sheet. Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculated scale according to PageSetup.FitToPagesWide and PageSetup.FitToPagesTall .

**Type:** Number

### getPageSizeInch(pageIndex) {#getpagesizeinch}

Get page size in inch of output image.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | The page index is based on zero. |

**Returns:** Page size of image, [0] for width and [1] for height

### toImage(pageIndex, fileName) {#toimage}

Render certain page to a file.

| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Number | indicate which page is to be converted |
| fileName | String | filename of the output image |

### toPrinter(printerName) (1 of 2) {#toprinter}

Render worksheet to Printer

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |

---

### toPrinter(printerName, jobName) (2 of 2) {#toprinter-1}

Render worksheet to Printer

| Parameter | Type | Description |
| --- | --- | --- |
| printerName | String | the name of the printer , for example: "Microsoft Office Document Image Writer" |
| jobName | String | set the print job name |
