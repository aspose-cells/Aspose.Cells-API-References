##PivotTable.SelectArea
PivotTable method. Select an area of pivot table view
## PivotTable.SelectArea method
Select an area of pivot table view.
```csharp
public PivotAreaCollection SelectArea(CellArea ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The cell area. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableMethodSelectAreaWithCellAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["B4"].Value = 3000;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Calculate data
pivotTable.CalculateData();
// Define the cell area to select
CellArea area = new CellArea();
area.StartRow = 2;
area.StartColumn = 4;
area.EndRow = 5;
area.EndColumn = 6;
try
{
// Call the SelectArea method with the CellArea parameter
PivotAreaCollection selectedAreas = pivotTable.SelectArea(area);
Console.WriteLine("SelectArea method executed successfully. Selected areas count: " + selectedAreas.Count);
// Save the workbook to show the effect
workbook.Save("PivotTableSelectAreaDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SelectArea method: {ex.Message}");
}
}
}
}
```
### See Also
* class [PivotAreaCollection](../../pivotareacollection/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
