---
title: Aspose::Cells::Pivot::PivotFieldTop10AutoShowSettings class
linktitle: PivotFieldTop10AutoShowSettings
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotFieldTop10AutoShowSettings class. Represents the Top 10 AutoShow settings for a pivot field in C++.'
type: docs
weight: 1900
url: /cpp/aspose.cells.pivot/pivotfieldtop10autoshowsettings/
---
## PivotFieldTop10AutoShowSettings class


Represents the Top 10 AutoShow settings for a pivot field.

```cpp
class PivotFieldTop10AutoShowSettings
```

## Methods

| Method | Description |
| --- | --- |
| [GetAutoShowCount()](./getautoshowcount/) | Represent the number of top or bottom items that are automatically shown in the specified [PivotTable](../pivottable/) field. |
| [GetRankBy()](./getrankby/) | Specifies the index of data field for AutoShow ranking. Represents auto show field index. -1 means [PivotField](../pivotfield/) itself. It should be the index of the data fields. |
| [IsAutoShow()](./isautoshow/) | Indicates whether an "Top 10 AutoShow" filter is applied to this field. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsTop()](./istop/) | Indicates whether the specified [PivotTable](../pivottable/) field is autoshown ascending. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotFieldTop10AutoShowSettings\& src)](./operator_asm/) | operator= |
| [PivotFieldTop10AutoShowSettings(PivotFieldTop10AutoShowSettings_Impl* impl)](./pivotfieldtop10autoshowsettings/) | Constructs from an implementation object. |
| [PivotFieldTop10AutoShowSettings(const PivotFieldTop10AutoShowSettings\& src)](./pivotfieldtop10autoshowsettings/) | Copy constructor. |
| [SetAutoShowCount(int32_t value)](./setautoshowcount/) | Represent the number of top or bottom items that are automatically shown in the specified [PivotTable](../pivottable/) field. |
| [SetIsAutoShow(bool value)](./setisautoshow/) | Indicates whether an "Top 10 AutoShow" filter is applied to this field. |
| [SetIsTop(bool value)](./setistop/) | Indicates whether the specified [PivotTable](../pivottable/) field is autoshown ascending. |
| [SetRankBy(int32_t value)](./setrankby/) | Specifies the index of data field for AutoShow ranking. Represents auto show field index. -1 means [PivotField](../pivotfield/) itself. It should be the index of the data fields. |
| [~PivotFieldTop10AutoShowSettings()](./~pivotfieldtop10autoshowsettings/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks


In xls : Implementing top 10 filters in Xls through Top 10 AutoShow In ooxml files: The underlying ooxml file format supports [Top10](../../aspose.cells/top10/) AutoShow, but Excel 2007 and later user interface only provides access via [Top10](../../aspose.cells/top10/) filter. If XLS compatibility is not required, it is recommended to use [Top10](../../aspose.cells/top10/) filter instead. 

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

//Show top 2 items by row field label.
rowField.Top10AutoShow(true, true, 2, -1);

PivotFieldTop10AutoShowSettings sortSetting = rowField.GetTop10AutoShowSettings();
//std::cout << sortSetting.IsAutoShow() << std::endl;

pivot.CalculateData();

book.Save("out.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
