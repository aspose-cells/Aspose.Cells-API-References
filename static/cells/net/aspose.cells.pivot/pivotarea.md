##Class PivotArea
Aspose.Cells.Pivot.PivotArea class. Presents the selected area of the PivotTable
## PivotArea class
Presents the selected area of the PivotTable.
```csharp
public class PivotArea
```
## Constructors
| Name | Description |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | Presents the selected area of the PivotTable. |
## Properties
| Name | Description |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | Gets and sets the region of the PivotTable to which this rule applies. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | Gets all filters for this PivotArea. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | Indicates whether the column grand total is included. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | Indicates whether the rule refers to an area that is in outline mode. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | Indicates whether the row grand total is included. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | Indicates whether only the data labels for an item selection are selected. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | Gets and sets the type of selection rule. |
## Methods
| Name | Description |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | Gets cell areas of this pivot area. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | Select the area with filters. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | Select a field in the region as an area. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | Select a field in the region as an area. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotAreaDemo
{
public static void PivotAreaExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells[0, 0].Value = "Fruit";
worksheet.Cells[1, 0].Value = "Apple";
worksheet.Cells[2, 0].Value = "Banana";
worksheet.Cells[3, 0].Value = "Cherry";
worksheet.Cells[0, 1].Value = "Year";
worksheet.Cells[1, 1].Value = 2020;
worksheet.Cells[2, 1].Value = 2021;
worksheet.Cells[3, 1].Value = 2022;
worksheet.Cells[0, 2].Value = "Amount";
worksheet.Cells[1, 2].Value = 50;
worksheet.Cells[2, 2].Value = 60;
worksheet.Cells[3, 2].Value = 70;
// Add a pivot table to the worksheet
int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount
// Create a PivotArea instance
PivotArea pivotArea = new PivotArea(pivotTable);
// Set properties of the PivotArea
pivotArea.OnlyData = true;
pivotArea.OnlyLabel = false;
pivotArea.IsRowGrandIncluded = true;
pivotArea.IsColumnGrandIncluded = true;
pivotArea.AxisType = PivotFieldType.Row;
pivotArea.RuleType = PivotAreaType.Normal;
pivotArea.IsOutline = false;
// Use the Select method to select a specific area
pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);
// Save the workbook
workbook.Save("PivotAreaExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
