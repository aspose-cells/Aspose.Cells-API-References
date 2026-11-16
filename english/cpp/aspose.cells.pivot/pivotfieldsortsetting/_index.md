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

## Examples


```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);
Cells cells = sheet.GetCells();
cells.Get(0, 0).PutValue(u"fruit");
cells.Get(1, 0).PutValue(u"grape");
cells.Get(2, 0).PutValue(u"blueberry");
cells.Get(3, 0).PutValue(u"kiwi");
cells.Get(4, 0).PutValue(u"cherry");
cells.Get(5, 0).PutValue(u"grape");
cells.Get(6, 0).PutValue(u"blueberry");
cells.Get(7, 0).PutValue(u"kiwi");
cells.Get(8, 0).PutValue(u"cherry");

cells.Get(0, 1).PutValue(u"year");
cells.Get(1, 1).PutValue(2020);
cells.Get(2, 1).PutValue(2020);
cells.Get(3, 1).PutValue(2020);
cells.Get(4, 1).PutValue(2020);
cells.Get(5, 1).PutValue(2021);
cells.Get(6, 1).PutValue(2021);
cells.Get(7, 1).PutValue(2021);
cells.Get(8, 1).PutValue(2021);

cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);
cells.Get(5, 2).PutValue(90);
cells.Get(6, 2).PutValue(100);
cells.Get(7, 2).PutValue(110);
cells.Get(8, 2).PutValue(120);

PivotTableCollection pivots = sheet.GetPivotTables();

PivotTable pivot = pivots.Add(u"=Sheet1!A1:C9", u"A12");

pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"year");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");

pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);

//Change PivotField's attributes
PivotField rowField = pivot.GetRowFields().Get(0);
rowField.SetDisplayName(u"custom display name");

//Sort by the first data field ascending.
rowField.SortBy(SortOrder::Ascending, 0, nullptr);

//Gets sort settings of the pivot field.
PivotFieldSortSetting sortSetting = rowField.GetSortSetting();
//std::cout << sortSetting.GetSortType() <<std::endl;

pivot.CalculateData();
book.Save("out.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
