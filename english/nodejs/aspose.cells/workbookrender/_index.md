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
| [getPageCount()](./getpagecount/) | Gets the total page count of workbook. |
| [getPageSizeInch(pageIndex)](./getpagesizeinch/) | Get page size in inch of output image. |
| [toImage(filename)](./toimage/) | Render whole workbook as Tiff Image to a file. |
| [toImage(pageIndex, fileName)](./toimage-1/) | Render certain page to a file. |
| [toImage(pageIndex, stream)](./toimage-2/) | Render certain page to a stream. |
| [toPrinter(printerName)](./toprinter/) | Render workbook to Printer |
| [toPrinter(printerName, jobName)](./toprinter-1/) | Render workbook to Printer |
| [toImageStream(workbookRender, stream)](./toimagestream/) *(static)* | Render whole workbook as Tiff Image to stream. |
