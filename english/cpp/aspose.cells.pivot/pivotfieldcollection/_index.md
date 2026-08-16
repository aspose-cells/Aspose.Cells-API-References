---
title: Aspose::Cells::Pivot::PivotFieldCollection class
linktitle: PivotFieldCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotFieldCollection class. Represents a collection of all the PivotField objects in the different regions of the pivot table in C++.'
type: docs
weight: 1400
url: /cpp/aspose.cells.pivot/pivotfieldcollection/
---
## PivotFieldCollection class


Represents a collection of all the [PivotField](../pivotfield/) objects in the different regions of the pivot table.

```cpp
class PivotFieldCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(const PivotField\& pivotField)](./add/) | Adds a [PivotField](../pivotfield/)[Object](../../aspose.cells/object/) to the specific type PivotFields. |
| [AddByBaseIndex(int32_t baseFieldIndex)](./addbybaseindex/) | Adds a [PivotField](../pivotfield/)[Object](../../aspose.cells/object/) to the specific type PivotFields. |
| [begin()](./begin/) | Returns an iterator to the beginning of the [PivotFieldCollection](./). |
| [Clear()](./clear/) | clear all fields of [PivotFieldCollection](./) |
| [end()](./end/) | Returns an iterator to the end of the [PivotFieldCollection](./). |
| [Get(int32_t index)](./get/) | Gets the [PivotField](../pivotfield/)[Object](../../aspose.cells/object/) at the specific index. |
| [Get(const U16String\& name)](./get/) | Gets the [PivotField](../pivotfield/)[Object](../../aspose.cells/object/) of the specific name. |
| [Get(const char16_t* name)](./get/) | Gets the [PivotField](../pivotfield/)[Object](../../aspose.cells/object/) of the specific name. |
| [GetCount()](./getcount/) | Gets the number of elements contained in the instance. |
| [GetType()](./gettype/) | Gets the PivotFields type. |
| [Insert(int32_t index, const PivotField\& pivotField)](./insert/) | Insert a pivot field at specific index. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [Move(int32_t currPos, int32_t destPos)](./move/) | Moves the [PivotField](../pivotfield/) from current position to destination position. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotFieldCollection\& src)](./operator_asm/) | operator= |
| [PivotFieldCollection(PivotFieldCollection_Impl* impl)](./pivotfieldcollection/) | Constructs from an implementation object. |
| [PivotFieldCollection(const PivotFieldCollection\& src)](./pivotfieldcollection/) | Copy constructor. |
| [Remove(const PivotField\& pivotField)](./remove/) | Removes field from the current region. |
| [RemoveAt(int32_t index)](./removeat/) | Removes field by the index. Only for filter,row,column,data region. |
| [~PivotFieldCollection()](./~pivotfieldcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
