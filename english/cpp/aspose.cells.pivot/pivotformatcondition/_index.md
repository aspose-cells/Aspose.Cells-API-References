---
title: Aspose::Cells::Pivot::PivotFormatCondition class
linktitle: PivotFormatCondition
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotFormatCondition class. Represents a PivotTable Format Condition in PivotFormatCondition Collection in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells.pivot/pivotformatcondition/
---
## PivotFormatCondition class


Represents a [PivotTable](../pivottable/) Format Condition in [PivotFormatCondition](./) Collection.

```cpp
class PivotFormatCondition
```

## Methods

| Method | Description |
| --- | --- |
| [AddColumnAreaCondition(const U16String\& fieldName)](./addcolumnareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the column fields. |
| [AddColumnAreaCondition(const char16_t* fieldName)](./addcolumnareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the column fields. |
| [AddColumnAreaCondition(const PivotField\& columnField)](./addcolumnareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the column fields. |
| [AddDataAreaCondition(const U16String\& fieldName)](./adddataareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the data fields. |
| [AddDataAreaCondition(const char16_t* fieldName)](./adddataareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the data fields. |
| [AddDataAreaCondition(const PivotField\& dataField)](./adddataareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the data fields. |
| [AddRowAreaCondition(const U16String\& fieldName)](./addrowareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the row fields. |
| [AddRowAreaCondition(const char16_t* fieldName)](./addrowareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the row fields. |
| [AddRowAreaCondition(const PivotField\& rowField)](./addrowareacondition/) | Adds [PivotTable](../pivottable/) conditional format limit in the row fields. |
| [GetFormatConditions()](./getformatconditions/) | Get formatconditions for the pivot table condition format . |
| [GetRuleType()](./getruletype/) | Get and set rule type for the pivot table condition format . |
| [GetScopeType()](./getscopetype/) | Get and set scope type for the pivot table condition format . |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotFormatCondition\& src)](./operator_asm/) | operator= |
| [PivotFormatCondition(PivotFormatCondition_Impl* impl)](./pivotformatcondition/) | Constructs from an implementation object. |
| [PivotFormatCondition(const PivotFormatCondition\& src)](./pivotformatcondition/) | Copy constructor. |
| [SetConditionalAreas()](./setconditionalareas/) | Sets conditional areas of [PivotFormatCondition](./) object. |
| [SetRuleType(PivotConditionFormatRuleType value)](./setruletype/) | Get and set rule type for the pivot table condition format . |
| [SetScopeType(PivotConditionFormatScopeType value)](./setscopetype/) | Get and set scope type for the pivot table condition format . |
| [~PivotFormatCondition()](./~pivotformatcondition/) | Destructor. |
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

//Add PivotFormatCondition
int formatIndex = pivot.GetPivotFormatConditions().Add();
PivotFormatCondition pfc = pivot.GetPivotFormatConditions().Get(formatIndex);
FormatConditionCollection fcc = pfc.GetFormatConditions();
fcc.AddArea(pivot.GetDataBodyRange());
int idx = fcc.AddCondition(FormatConditionType::CellValue);
FormatCondition fc = fcc.Get(idx);
fc.SetFormula1(u"100");
fc.SetOperator(OperatorType::GreaterOrEqual);
fc.GetStyle().SetBackgroundColor(Color{ 0xff, 0xff, 0, 0 });//Red

pivot.RefreshData();
pivot.CalculateData();


book.Save("out.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
