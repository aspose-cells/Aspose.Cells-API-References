---
title: RowCollection Class 
linktitle: RowCollection
second_title: Aspose.Cells for Go API Reference
description: 'RowCollection class. Encapsulates the object that represents rowcollection in Go.'
type: docs
weight: 200
url: /go/aspose.cells/rowcollection/
---

## RowCollection class

Collects the <see cref="Row"/> objects that represent the individual rows in a worksheet.

```go

type RowCollection struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetCount](./getcount/) | Gets the number of rows in this collection. | 
|[GetRowByIndex](./getrowbyindex/) | Gets the row object by the position in the list. | 
|[Get](./get/) | Gets a <see cref="Row"/> object by given row index. The Row object of given row index will be instantiated if it does not exist before. | 
|[Clear](./clear/) | Clear all rows and cells. | 
|[RemoveAt](./removeat/) | Remove the row item at the specified index(position) in this collection. | 
