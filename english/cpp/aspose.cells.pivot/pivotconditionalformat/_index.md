---
title: Aspose::Cells::Pivot::PivotConditionalFormat class
linktitle: PivotConditionalFormat
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotConditionalFormat class. Represents the conditional format of pivot table in C++.'
type: docs
weight: 1000
url: /cpp/aspose.cells.pivot/pivotconditionalformat/
---
## PivotConditionalFormat class


Represents the conditional format of pivot table.

```cpp
class PivotConditionalFormat
```

## Methods

| Method | Description |
| --- | --- |
| [AddCellArea(const CellArea\& ca)](./addcellarea/) | Adds an area based on pivot table view. |
| [AddFieldArea(PivotFieldType axisType, const U16String\& fieldName)](./addfieldarea/) | Adds an area of pivot field. |
| [AddFieldArea(PivotFieldType axisType, const char16_t* fieldName)](./addfieldarea/) | Adds an area of pivot field. |
| [AddFieldArea(PivotFieldType axisType, const PivotField\& field)](./addfieldarea/) | Adds an area of pivot field. |
| [ApplyTo(int32_t row, int32_t column, PivotConditionFormatScopeType scope)](./applyto/) | Applies the conditional format to range which must in data region. |
| [GetCellAreas()](./getcellareas/) | Gets all cell areas where this conditional format applies to. |
| [GetFormatConditions()](./getformatconditions/) | Get conditions for the pivot table conditional format . |
| [GetPivotAreas()](./getpivotareas/) | Gets all pivot areas. |
| [GetRuleType()](./getruletype/) | Get and set rule type for the pivot table condition format . |
| [GetScopeType()](./getscopetype/) | Get and set scope type for the pivot table conditional format . |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotConditionalFormat\& src)](./operator_asm/) | operator= |
| [PivotConditionalFormat(PivotConditionalFormat_Impl* impl)](./pivotconditionalformat/) | Constructs from an implementation object. |
| [PivotConditionalFormat(const PivotConditionalFormat\& src)](./pivotconditionalformat/) | Copy constructor. |
| [SetRuleType(PivotConditionFormatRuleType value)](./setruletype/) | Get and set rule type for the pivot table condition format . |
| [SetScopeType(PivotConditionFormatScopeType value)](./setscopetype/) | Get and set scope type for the pivot table conditional format . |
| [~PivotConditionalFormat()](./~pivotconditionalformat/) | Destructor. |
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

//Add PivotFormatCondition
int formatIndex = pivot.GetConditionalFormats().Add();
PivotConditionalFormat pfc = pivot.GetConditionalFormats().Get(formatIndex);
pfc.AddCellArea(pivot.GetDataBodyRange());
FormatConditionCollection fcc = pfc.GetFormatConditions();
int ii = fcc.AddCondition(FormatConditionType::CellValue, OperatorType::GreaterOrEqual, u"100", nullptr);

FormatCondition fc = fcc.Get(ii);
fc.GetStyle().SetBackgroundColor(Color::Red());
pivot.CalculateData();


book.Save("out.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
