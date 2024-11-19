---
title: FormatConditionCollection Class 
linktitle: FormatConditionCollection
second_title: Aspose.Cells for Go API Reference
description: 'FormatConditionCollection class. Encapsulates the object that represents formatconditioncollection in Go.'
type: docs
weight: 200
url: /go/aspose.cells/formatconditioncollection/
---

## FormatConditionCollection class

Represents conditional formatting.The FormatConditions can contain up to three conditional formats.

```go

type FormatConditionCollection struct 

formatconditioncollection, _ := asposecells.NewFormatConditionCollection()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewFormatConditionCollection](./newformatconditioncollection/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[AddArea](./addarea/) | Adds a conditional formatted cell range. | 
|[AddCondition](./addcondition/) | Adds a formatting condition. | 
|[AddCondition](./addcondition/) | Add a format condition. | 
|[GetCount](./getcount/) | Gets the count of the conditions. | 
|[GetRangeCount](./getrangecount/) | Gets count of conditionally formatted ranges. | 
|[Get](./get/) | Gets the formatting condition by index. | 
|[GetCellArea](./getcellarea/) | Gets the conditional formatted cell range by index. | 
|[RemoveArea](./removearea/) | Removes conditional formatted cell range by index. | 
|[RemoveArea](./removearea/) | Remove conditional formatting int the range. | 
|[RemoveCondition](./removecondition/) | Removes the formatting condition by index. | 
