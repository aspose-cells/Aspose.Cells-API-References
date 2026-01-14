---
title: Slicer Class 
linktitle: Slicer
second_title: Aspose.Cells for Go via C++ API Reference
description: 'Slicer class. Encapsulates the object that represents slicer in Go.'
type: docs
weight: 200
url: /go-cpp/slicer/
---

## Slicer class

summary description of Slicer View

```go

type Slicer struct  {
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
|[GetSortOrderType](./getsortordertype/) | Indicates the type of sorting items. | 
|[SetSortOrderType](./setsortordertype/) | Indicates the type of sorting items. | 
|[GetShowMissing](./getshowmissing/) | Indicates whether to show items deteleted from the data source. | 
|[SetShowMissing](./setshowmissing/) | Indicates whether to show items deteleted from the data source. | 
|[GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | Indicates whether to show items deteleted from the data source. | 
|[SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | Indicates whether to show items deteleted from the data source. | 
|[GetShowAllItems](./getshowallitems/) | Indicates whether to show all items even if there are no data or they are deleted.Default value is true; | 
|[SetShowAllItems](./setshowallitems/) | Indicates whether to show all items even if there are no data or they are deleted.Default value is true; | 
|[AddPivotConnection](./addpivotconnection/) | Adds PivotTable connection. | 
|[RemovePivotConnection](./removepivotconnection/) | Removes PivotTable connection. | 
|[GetLockedPosition](./getlockedposition/) | Indicates whether the specified slicer can be moved or resized by using the user interface. | 
|[SetLockedPosition](./setlockedposition/) | Indicates whether the specified slicer can be moved or resized by using the user interface. | 
|[Refresh](./refresh/) | Refreshing the slicer.Meanwhile, Refreshing and Calculating PivotTables which this slicer based on. | 
|[GetShape](./getshape/) | Returns the Shape object associated with the specified slicer. Read-only. | 
|[GetSlicerCache](./getslicercache/) | Returns the SlicerCache object associated with the slicer. Read-only. | 
|[GetWorksheet](./getworksheet/) | Returns the Worksheet object which contains this slicer. Read-only. | 
|[GetStyleType](./getstyletype/) | Specify the type of Built-in slicer style.The default type is SlicerStyleLight1. | 
|[SetStyleType](./setstyletype/) | Specify the type of Built-in slicer style.The default type is SlicerStyleLight1. | 
|[GetName](./getname/) | Returns or sets the name of the specified slicer | 
|[SetName](./setname/) | Returns or sets the name of the specified slicer | 
|[GetCaption](./getcaption/) | Returns or sets the caption of the specified slicer. | 
|[SetCaption](./setcaption/) | Returns or sets the caption of the specified slicer. | 
|[GetFirstItemIndex](./getfirstitemindex/) | Specifies the zero-based index of the first slicer item. | 
|[SetFirstItemIndex](./setfirstitemindex/) | Specifies the zero-based index of the first slicer item. | 
|[GetShowCaption](./getshowcaption/) | Indicates whether the header of the slicer is visible.The default value is true | 
|[SetShowCaption](./setshowcaption/) | Indicates whether the header of the slicer is visible.The default value is true | 
|[GetNumberOfColumns](./getnumberofcolumns/) | Returns or sets the number of columns in the specified slicer.The default value is 1. | 
|[SetNumberOfColumns](./setnumberofcolumns/) | Returns or sets the number of columns in the specified slicer.The default value is 1. | 
|[GetColumnWidthPixel](./getcolumnwidthpixel/) | Gets or sets the width of each column in the slicer, in unit of pixels. | 
|[SetColumnWidthPixel](./setcolumnwidthpixel/) | Gets or sets the width of each column in the slicer, in unit of pixels. | 
|[GetColumnWidth](./getcolumnwidth/) | Returns or sets the width of each column in the slicer in unit of points. | 
|[SetColumnWidth](./setcolumnwidth/) | Returns or sets the width of each column in the slicer in unit of points. | 
|[GetRowHeightPixel](./getrowheightpixel/) | Returns or sets the height of each row in the specified slicer, in unit of pixels. | 
|[SetRowHeightPixel](./setrowheightpixel/) | Returns or sets the height of each row in the specified slicer, in unit of pixels. | 
|[GetRowHeight](./getrowheight/) | Returns or sets the height of each row in the specified slicer in unit of points. | 
|[SetRowHeight](./setrowheight/) | Returns or sets the height of each row in the specified slicer in unit of points. | 
