---
title: WorkbookRender Class 
linktitle: WorkbookRender
second_title: Aspose.Cells for Go API Reference
description: 'WorkbookRender class. Encapsulates the object that represents workbookrender in Go.'
type: docs
weight: 200
url: /go/aspose.cells.rendering/workbookrender/
---

## WorkbookRender class

Represents a Workbook render.The constructor of this class , must be used after modification of pagesetup, cell style.

```go

type WorkbookRender struct 

workbookrender, _ := asposecells.NewWorkbookRender()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewWorkbookRender_Workbook_ImageOrPrintOptions](./newworkbookrender_workbook_imageorprintoptions/) | The construct of WorkbookRender | 
|[NewWorkbookRender_WorkbookRender](./newworkbookrender_workbookrender/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetPageCount](./getpagecount/) | Gets the total page count of workbook. | 
|[ToImage](./toimage/) | Render whole workbook as Tiff Image to a file. | 
|[ToImage](./toimage/) | Render certain page to a file. | 
|[Dispose](./dispose/) | Releases resources created and used for rendering. | 
