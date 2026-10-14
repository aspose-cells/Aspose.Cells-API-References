---
title: PivotFieldCollection Class 
linktitle: PivotFieldCollection
second_title: Aspose.Cells for Go via C++ API Reference
description: 'PivotFieldCollection class. Encapsulates the object that represents pivotfieldcollection in Go.'
type: docs
weight: 200
url: /go-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

Represents a collection of all the PivotField objects in the different regions of the pivot table.

```go

type PivotFieldCollection struct  {
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
|[GetType](./gettype/) | Gets the PivotFields type. | 
|[Get_Int](./get_int/) | Gets the PivotField Object at the specific index. | 
|[Get_String](./get_string/) | Gets the PivotField Object of the specific name. | 
|[RemoveAt](./removeat/) | Removes field by the index.Only for filter,row,column,data region. | 
|[AddByBaseIndex](./addbybaseindex/) | Adds a PivotField Object to the specific type PivotFields. | 
|[Add](./add/) | Adds a PivotField Object to the specific type PivotFields. | 
|[Insert](./insert/) | Insert a pivot field at specific index. | 
|[Clear](./clear/) | clear all fields of PivotFieldCollection | 
|[Remove](./remove/) | Removes field from the current region. | 
|[Move](./move/) | Moves the PivotField from current position to destination position | 
|[GetCount](./getcount/) | Gets the number of elements contained in the instance. | 
