---
title: Aspose::Cells::Timelines::TimelineCollection class
linktitle: TimelineCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Timelines::TimelineCollection class. Specifies the collection of all the Timeline objects on the worksheet. It was supported since Excel 2013 in C++.'
type: docs
weight: 200
url: /cpp/aspose.cells.timelines/timelinecollection/
---
## TimelineCollection class


Specifies the collection of all the [Timeline](../timeline/) objects on the worksheet. It was supported since Excel 2013.

```cpp
class TimelineCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(const PivotTable\& pivot, int32_t row, int32_t column, const U16String\& baseFieldName)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, int32_t row, int32_t column, const char16_t* baseFieldName)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const U16String\& destCellName, const U16String\& baseFieldName)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const char16_t* destCellName, const char16_t* baseFieldName)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, int32_t row, int32_t column, int32_t baseFieldIndex)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const U16String\& destCellName, int32_t baseFieldIndex)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const char16_t* destCellName, int32_t baseFieldIndex)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, int32_t row, int32_t column, const PivotField\& baseField)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const U16String\& destCellName, const PivotField\& baseField)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Add(const PivotTable\& pivot, const char16_t* destCellName, const PivotField\& baseField)](./add/) | Add a new [Timeline](../timeline/) using PivotTable as data source. |
| [Get(int32_t index)](./get/) | Gets the [Timeline](../timeline/) by index. |
| [Get(const U16String\& name)](./get/) | Gets the [Timeline](../timeline/) by [Timeline](../timeline/)'s name. |
| [Get(const char16_t* name)](./get/) | Gets the [Timeline](../timeline/) by [Timeline](../timeline/)'s name. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TimelineCollection\& src)](./operator_asm/) | operator= |
| [TimelineCollection(TimelineCollection_Impl* impl)](./timelinecollection/) | Constructs from an implementation object. |
| [TimelineCollection(const TimelineCollection\& src)](./timelinecollection/) | Copy constructor. |
| [~TimelineCollection()](./~timelinecollection/) | Destructor. |
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

//Create date style
Style dateStyle = CellsFactory().CreateStyle();
dateStyle.SetCustom(u"m/d/yyyy");
cells.Get(0, 1).PutValue(u"date");
cells.Get(1, 1).PutValue(Date{ 2021, 2, 5 });
cells.Get(2, 1).PutValue(Date{ 2022, 3, 8 });
cells.Get(3, 1).PutValue(Date{ 2023, 4, 10 });
cells.Get(4, 1).PutValue(Date{ 2024, 5, 16 });
//Set date style
cells.Get(1, 1).SetStyle(dateStyle);
cells.Get(2, 1).SetStyle(dateStyle);
cells.Get(3, 1).SetStyle(dateStyle);
cells.Get(4, 1).SetStyle(dateStyle);

cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);

PivotTableCollection pivots = sheet.GetPivotTables();
//Add a PivotTable
int pivotIndex = pivots.Add(u"=Sheet1!A1:C5", u"A12", u"TestPivotTable");
PivotTable pivot = pivots.Get(pivotIndex);
pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"date");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");
pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);

//Refresh PivotTable data
pivot.RefreshData();
pivot.CalculateData();

book.Save("out.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Timelines](../)
* Library [Aspose.Cells for C++](../../)
