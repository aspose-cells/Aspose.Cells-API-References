---
title: Class PivotConditionalFormat
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotConditionalFormat class. Represents a PivotTable Format Condition in PivotFormatCondition Collection
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/
---
## PivotConditionalFormat class

Represents a PivotTable Format Condition in PivotFormatCondition Collection.

```csharp
public class PivotConditionalFormat
```

## Properties

| Name | Description |
| --- | --- |
| [FormatConditions](../../aspose.cells.pivot/pivotconditionalformat/formatconditions/) { get; } | Get conditions for the pivot table conditional format . |
| [PivotAreas](../../aspose.cells.pivot/pivotconditionalformat/pivotareas/) { get; } | Gets all pivot areas. |
| [RuleType](../../aspose.cells.pivot/pivotconditionalformat/ruletype/) { get; set; } | Get and set rule type for the pivot table condition format . |
| [ScopeType](../../aspose.cells.pivot/pivotconditionalformat/scopetype/) { get; set; } | Get and set scope type for the pivot table conditional format . |

## Methods

| Name | Description |
| --- | --- |
| [AddCellArea](../../aspose.cells.pivot/pivotconditionalformat/addcellarea/)(CellArea) | Adds an area based on pivot table view. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea)(PivotFieldType, PivotField) | Adds an area of pivot field. |
| [AddFieldArea](../../aspose.cells.pivot/pivotconditionalformat/addfieldarea/#addfieldarea_1)(PivotFieldType, string) | Adds an area of pivot field. |
| [ApplyTo](../../aspose.cells.pivot/pivotconditionalformat/applyto/)(int, int, PivotConditionFormatScopeType) | Applies the conditional format to range. Only for the data region. |
| [GetCellAreas](../../aspose.cells.pivot/pivotconditionalformat/getcellareas/)() | Gets all cell areas where this conditional format applies to. |

### Examples

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Add PivotFormatCondition
int formatIndex = pivot.ConditionalFormats.Add();
PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
pfc.AddFieldArea(PivotFieldType.Data, pivot.DataFields[0]);
int idx = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = pfc.FormatConditions[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

//do your business

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Add PivotFormatCondition
Dim formatIndex As Int32 = pivot.ConditionalFormats.Add()
Dim pfc As PivotConditionalFormat = pivot.ConditionalFormats(formatIndex)
pfc.AddFieldArea(PivotFieldType.Data, pivot.DataFields(0))
Dim idx As Int32 = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = pfc.FormatConditions(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


