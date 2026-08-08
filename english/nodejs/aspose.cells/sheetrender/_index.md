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
| [getPageCount()](./getpagecount/) | Gets the total page count of current worksheet. |
| [getPageScale()](./getpagescale/) | Gets calculated page scale of the sheet. Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculat |
| [getPageSizeInch(pageIndex)](./getpagesizeinch/) | Get page size in inch of output image. |
| [toImage(pageIndex, fileName)](./toimage/) | Render certain page to a file. |
| [toPrinter(printerName)](./toprinter/) | Render worksheet to Printer |
| [toPrinter(printerName, jobName)](./toprinter-1/) | Render worksheet to Printer |
| [toImageStream(sheetRender, pageIndex, stream)](./toimagestream/) *(static)* | Render certain page to a stream. |
