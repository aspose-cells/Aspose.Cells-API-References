##Class PivotConditionalFormat
Aspose.Cells.Pivot.PivotConditionalFormat class. Represents a PivotTable Format Condition in PivotFormatCondition Collection
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
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PivotClassPivotConditionalFormatDemo
{
public static void Run()
{
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
// Set sample data
cells["A1"].Value = "fruit";
cells["A2"].Value = "grape";
cells["A3"].Value = "blueberry";
cells["A4"].Value = "kiwi";
cells["A5"].Value = "cherry";
cells["A6"].Value = "grape";
cells["A7"].Value = "blueberry";
cells["A8"].Value = "kiwi";
cells["A9"].Value = "cherry";
cells["B1"].Value = "year";
cells["B2"].Value = 2020;
cells["B3"].Value = 2020;
cells["B4"].Value = 2020;
cells["B5"].Value = 2020;
cells["B6"].Value = 2021;
cells["B7"].Value = 2021;
cells["B8"].Value = 2021;
cells["B9"].Value = 2021;
cells["C1"].Value = "amount";
cells["C2"].Value = 50;
cells["C3"].Value = 60;
cells["C4"].Value = 70;
cells["C5"].Value = 80;
cells["C6"].Value = 90;
cells["C7"].Value = 100;
cells["C8"].Value = 110;
cells["C9"].Value = 120;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("=A1:C9", "A12", "TestPivotTable");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
// Add conditional formatting
int formatIndex = pivot.ConditionalFormats.Add();
PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
pfc.AddFieldArea(PivotFieldType.Data, pivot.DataFields[0]);
int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = pfc.FormatConditions[conditionIndex];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;
pivot.RefreshData();
book.Save("PivotConditionalFormatDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
