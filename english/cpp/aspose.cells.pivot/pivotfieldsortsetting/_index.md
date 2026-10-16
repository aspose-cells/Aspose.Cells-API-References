---
title: Aspose::Cells::Pivot::PivotFieldSortSetting class
linktitle: PivotFieldSortSetting
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotFieldSortSetting class. Represents the setting for sorting pivot fields in C++.'
type: docs
weight: 1800
url: /cpp/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class


Represents the setting for sorting pivot fields.

```cpp
class PivotFieldSortSetting
```

## Methods

| Method | Description |
| --- | --- |
| [GetCell()](./getcell/) | Sorts by the values in which row or column. |
| [GetFieldIndex()](./getfieldindex/) |  **(Deprecated)** Represents the index of the field sorted by. -1 means sorting the [PivotField](../pivotfield/) by the labels,others means sorting by the data field. |
| [GetLineTypeSortedBy()](./getlinetypesortedby/) | The pivot line type sorted by. |
| [GetSortBy()](./getsortby/) | Represents the index of the field sorted by. A value of -1 indicates sorting by the pivot item's own values. When greater than or equal to zero, it represents the index of data field in the data region. |
| [GetSortType()](./getsorttype/) | Represents the [SortOrder](../../aspose.cells/sortorder/). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsSimpleSort()](./issimplesort/) | Indicates whether a simple data sort operation will be applied. |
| [IsSortByLabels()](./issortbylabels/) | Indicates whether to sort the field by itself or data field. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotFieldSortSetting\& src)](./operator_asm/) | operator= |
| [PivotFieldSortSetting(PivotFieldSortSetting_Impl* impl)](./pivotfieldsortsetting/) | Constructs from an implementation object. |
| [PivotFieldSortSetting(const PivotFieldSortSetting\& src)](./pivotfieldsortsetting/) | Copy constructor. |
| [SetFieldIndex(int32_t value)](./setfieldindex/) |  **(Deprecated)** Represents the index of the field sorted by. -1 means sorting the [PivotField](../pivotfield/) by the labels,others means sorting by the data field. |
| [SetIsSimpleSort(bool value)](./setissimplesort/) | Indicates whether a simple data sort operation will be applied. |
| [SetSortBy(int32_t value)](./setsortby/) | Represents the index of the field sorted by. A value of -1 indicates sorting by the pivot item's own values. When greater than or equal to zero, it represents the index of data field in the data region. |
| [SetSortType(SortOrder value)](./setsorttype/) | Represents the [SortOrder](../../aspose.cells/sortorder/). |
| [~PivotFieldSortSetting()](./~pivotfieldsortsetting/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
