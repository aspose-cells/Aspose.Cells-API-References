##PivotArea.GetCellAreas
PivotArea method. Gets cell areas of this pivot area
## PivotArea.GetCellAreas method
Gets cell areas of this pivot area.
```csharp
public CellArea[] GetCellAreas()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotAreaMethodGetCellAreasDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create minimal pivot table data
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "Fruit";
worksheet.Cells["A3"].Value = "Vegetable";
try
{
// Create pivot table with basic configuration
int pivotIndex = worksheet.PivotTables.Add("A1:A3", "D1", "DemoPivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Initialize pivot area with the pivot table instance
PivotArea pivotArea = new PivotArea(pivotTable);
// Configure pivot area settings
pivotArea.RuleType = PivotAreaType.Normal;
pivotArea.AxisType = PivotFieldType.Data;
pivotArea.IsRowGrandIncluded = true;
// Execute target method
CellArea[] cellAreas = pivotArea.GetCellAreas();
Console.WriteLine($"GetCellAreas returned {cellAreas.Length} cell area(s)");
foreach (CellArea area in cellAreas)
{
Console.WriteLine($"CellArea: Columns {area.StartColumn}-{area.EndColumn}, Rows {area.StartRow}-{area.EndRow}");
}
workbook.Save("GetCellAreasDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error calling GetCellAreas: {ex.Message}");
}
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
