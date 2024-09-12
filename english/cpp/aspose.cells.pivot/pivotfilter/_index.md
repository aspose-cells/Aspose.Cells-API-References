---
title: Aspose::Cells::Pivot::PivotFilter class
linktitle: PivotFilter
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotFilter class. Represents a PivotFilter in PivotFilter Collection in C++.'
type: docs
weight: 1100
url: /cpp/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class


Represents a [PivotFilter](./) in [PivotFilter](./) Collection.

```cpp
class PivotFilter
```

## Methods

| Method | Description |
| --- | --- |
| [GetAutoFilter()](./getautofilter/) | Gets the autofilter of the pivot filter. |
| [GetEvaluationOrder()](./getevaluationorder/) | Gets the Evaluation Order of the pivot filter. |
| [GetFieldIndex()](./getfieldindex/) | Gets the field index of the pivot filter. |
| [GetFilterType()](./getfiltertype/) | Gets the autofilter type of the pivot filter. |
| [GetMeasureFldIndex()](./getmeasurefldindex/) | Gets the measure field index of the pivot filter. |
| [GetMemberPropertyFieldIndex()](./getmemberpropertyfieldindex/) | Gets the member property field index of the pivot filter. |
| [GetName()](./getname/) | Gets the name of the pivot filter. |
| [GetValue1()](./getvalue1/) | Gets the string value1 of the label pivot filter. |
| [GetValue2()](./getvalue2/) | Gets the string value2 of the label pivot filter. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotFilter\& src)](./operator_asm/) | operator= |
| [PivotFilter(PivotFilter_Impl* impl)](./pivotfilter/) | Constructs from an implementation object. |
| [PivotFilter(const PivotFilter\& src)](./pivotfilter/) | Copy constructor. |
| [SetEvaluationOrder(int32_t value)](./setevaluationorder/) | Gets the Evaluation Order of the pivot filter. |
| [SetMeasureFldIndex(int32_t value)](./setmeasurefldindex/) | Gets the measure field index of the pivot filter. |
| [SetMemberPropertyFieldIndex(int32_t value)](./setmemberpropertyfieldindex/) | Gets the member property field index of the pivot filter. |
| [SetName(const U16String\& value)](./setname/) | Gets the name of the pivot filter. |
| [SetName(const char16_t* value)](./setname/) | Gets the name of the pivot filter. |
| [SetValue1(const U16String\& value)](./setvalue1/) | Gets the string value1 of the label pivot filter. |
| [SetValue1(const char16_t* value)](./setvalue1/) | Gets the string value1 of the label pivot filter. |
| [SetValue2(const U16String\& value)](./setvalue2/) | Gets the string value2 of the label pivot filter. |
| [SetValue2(const char16_t* value)](./setvalue2/) | Gets the string value2 of the label pivot filter. |
| [~PivotFilter()](./~pivotfilter/) | Destructor. |
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

int pivotIndex = pivots.Add(u"=Sheet1!A1:C9", u"A12", u"TestPivotTable");
PivotTable pivot = pivots.Get(pivotIndex);
pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"year");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");

pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);

//Add PivotFilter
int index = pivot.GetPivotFilters().Add(0, PivotFilterType::Count);
PivotFilter filter = pivot.GetPivotFilters().Get(index);
filter.GetAutoFilter().FilterTop10(0, false, false, 2);

pivot.RefreshData();
pivot.CalculateData();


book.Save("out.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
