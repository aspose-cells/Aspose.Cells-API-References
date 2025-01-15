---
title: SheetRender Class 
linktitle: SheetRender
second_title: Aspose.Cells for Go via C++ API Reference
description: 'SheetRender class. Encapsulates the object that represents sheetrender in Go.'
type: docs
weight: 200
url: /go-cpp/sheetrender/
---

## SheetRender class

Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..)The constructor of this class , must be used after modification of pagesetup, cell style.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewSheetRender](./newsheetrender/) | the construct of SheetRender, need worksheet and ImageOrPrintOptions as params | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetPageCount](./getpagecount/) | Gets the total page count of current worksheet. | 
|[GetPageScale](./getpagescale/) | Gets calculated page scale of the sheet.Returns the set scale if PageSetup.Zoom is set. Otherwise, returns the calculated scale according to PageSetup.FitToPagesWide and PageSetup.FitToPagesTall. | 
|[GetPageSizeInch](./getpagesizeinch/) | Get page size in inch of output image. | 
|[ToImage_Int_String](./toimage_int_string/) | Render certain page to a file. | 
|[ToImage_Int](./toimage_int/) | Render certain page to a stream. | 
|[ToTiff_Stream](./totiff_stream/) | Render whole worksheet as Tiff Image to stream. | 
|[ToTiff_String](./totiff_string/) | Render whole worksheet as Tiff Image to a file. | 
|[Dispose](./dispose/) | Releases resources created and used for rendering. | 
