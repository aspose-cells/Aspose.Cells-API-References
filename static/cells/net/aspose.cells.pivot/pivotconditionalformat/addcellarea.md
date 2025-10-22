##PivotConditionalFormat.AddCellArea
PivotConditionalFormat method. Adds an area based on pivot table view
## PivotConditionalFormat.AddCellArea method
Adds an area based on pivot table view.
```csharp
public void AddCellArea(CellArea ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The cell area. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotConditionalFormatMethodAddCellAreaWithCellAreaDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["A3"].Value = "Orange";
cells["A4"].Value = "Banana";
cells["B2"].Value = 120;
cells["B3"].Value = 85;
cells["B4"].Value = 90;
// Add pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Create a cell area for conditional formatting
CellArea cellArea = new CellArea();
cellArea.StartRow = 4;
cellArea.StartColumn = 5;
cellArea.EndRow = 6;
cellArea.EndColumn = 7;
// Add conditional format with cell area
int formatIndex = pivotTable.ConditionalFormats.Add();
PivotConditionalFormat pcf = pivotTable.ConditionalFormats[formatIndex];
pcf.AddCellArea(cellArea);
// Add format condition
int conditionIndex = pcf.FormatConditions.AddCondition(FormatConditionType.CellValue);
FormatCondition condition = pcf.FormatConditions[conditionIndex];
condition.Formula1 = "50";
condition.Operator = OperatorType.GreaterOrEqual;
condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;
// Calculate pivot table data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotConditionalFormatWithCellArea.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
