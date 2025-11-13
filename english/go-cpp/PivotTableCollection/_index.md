---
title: PivotTableCollection Class 
linktitle: PivotTableCollection
second_title: Aspose.Cells for Go via C++ API Reference
description: 'PivotTableCollection class. Encapsulates the object that represents pivottablecollection in Go.'
type: docs
weight: 200
url: /go-cpp/pivottablecollection/
---

## PivotTableCollection class

Represents the collection of all the PivotTable objects on the specified worksheet.

```go

type PivotTableCollection struct  {
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
|[Dispose](./dispose/) | Performs application-defined tasks associated with freeing, releasing, orresetting unmanaged resources. | 
|[Add_String_String_String](./add_string_string_string/) | Adds a new PivotTable. | 
|[Add_String_String_String_Bool](./add_string_string_string_bool/) | Adds a new PivotTable. | 
|[Add_String_Int_Int_String](./add_string_int_int_string/) | Adds a new PivotTable. | 
|[Add_String_Int_Int_String_Bool](./add_string_int_int_string_bool/) | Adds a new PivotTable. | 
|[Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | Adds a new PivotTable. | 
|[Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | Adds a new PivotTable. | 
|[Add_PivotTable_String_String](./add_pivottable_string_string/) | Adds a new PivotTable based on another PivotTable. | 
|[Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Adds a new PivotTable based on another PivotTable. | 
|[Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. | 
|[Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. | 
|[Get_Int](./get_int/) | Gets the PivotTable report by index. | 
|[Get_String](./get_string/) | Gets the PivotTable report by pivottable's name. | 
|[Get_Int_Int](./get_int_int/) | Gets the PivotTable report by pivottable's position. | 
|[Clear](./clear/) | Clears all pivot tables. | 
|[Remove_PivotTable](./remove_pivottable/) | Deletes the specified PivotTable and delete the PivotTable data | 
|[Remove_PivotTable_Bool](./remove_pivottable_bool/) | Deletes the specified PivotTable | 
|[RemoveAt_Int](./removeat_int/) | Deletes the PivotTable at the specified index and delete the PivotTable data | 
|[RemoveAt_Int_Bool](./removeat_int_bool/) | Deletes the PivotTable at the specified index | 
|[GetCount](./getcount/) |  | 
