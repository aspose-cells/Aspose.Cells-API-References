---
title: PivotItem Class 
linktitle: PivotItem
second_title: Aspose.Cells for Go via C++ API Reference
description: 'PivotItem class. Encapsulates the object that represents pivotitem in Go.'
type: docs
weight: 200
url: /go-cpp/pivotitem/
---

## PivotItem class

Represents a item in a PivotField report.

```go

type PivotItem struct  {
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
|[IsHidden](./ishidden/) | Gets and Sets whether the pivot item is hidden. | 
|[SetIsHidden](./setishidden/) | Gets and Sets whether the pivot item is hidden. | 
|[GetPosition](./getposition/) | Specifying the index of this item in all the PivotItems of the field. | 
|[SetPosition](./setposition/) | Specifying the index of this item in all the PivotItems of the field. | 
|[GetPositionInSameParentNode](./getpositioninsameparentnode/) | Specifying the position index in the PivotItems under the same parent node. | 
|[SetPositionInSameParentNode](./setpositioninsameparentnode/) | Specifying the position index in the PivotItems under the same parent node. | 
|[Move](./move/) | Moves the item up or down | 
|[IsDetailHidden](./isdetailhidden/) | Gets and sets whether the detail of this pivot item is hidden. | 
|[SetIsDetailHidden](./setisdetailhidden/) | Gets and sets whether the detail of this pivot item is hidden. | 
|[IsCalculatedItem](./iscalculateditem/) | Indicates whether this pivot item is a calculated formula item. | 
|[GetFormula](./getformula/) | Gets the formula of this calculated item.Only works when this item is a calculated item. | 
|[IsMissing](./ismissing/) | Indicates whether the item was removed from the data source. | 
|[GetStringValue](./getstringvalue/) | Gets the string value of the pivot itemIf the value is null, it will return "" | 
|[GetDoubleValue](./getdoublevalue/) | Gets the double value of the pivot itemIf the value is null or not number ,it will return 0 | 
|[GetDateTimeValue](./getdatetimevalue/) | Gets the date time value of the pivot itemIf the value is null ,it will return DateTime.MinValue | 
|[GetValue](./getvalue/) | Gets the value of the pivot item | 
|[GetName](./getname/) | Gets the name of the pivot item. | 
|[SetName](./setname/) | Gets the name of the pivot item. | 
