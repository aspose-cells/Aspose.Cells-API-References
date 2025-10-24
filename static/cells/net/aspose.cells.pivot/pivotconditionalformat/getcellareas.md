##PivotConditionalFormat.GetCellAreas
PivotConditionalFormat method. Gets all cell areas where this conditional format applies to
## PivotConditionalFormat.GetCellAreas method
Gets all cell areas where this conditional format applies to.
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
public class PivotConditionalFormatMethodGetCellAreasDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create a pivot table required for PivotConditionalFormat
worksheet.Cells["A1"].Value = "Header";
worksheet.Cells["A2"].Value = "Data";
int pivotIndex = worksheet.PivotTables.Add("A1:A2", "B3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Create conditional format through pivot table's collection
int formatIndex = pivotTable.ConditionalFormats.Add();
PivotConditionalFormat conditionalFormat = pivotTable.ConditionalFormats[formatIndex];
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 2;
area.EndColumn = 2;
conditionalFormat.AddCellArea(area);
CellArea[] resultAreas = conditionalFormat.GetCellAreas();
Console.WriteLine($"Retrieved {resultAreas.Length} cell area(s):");
foreach (CellArea ca in resultAreas)
{
Console.WriteLine($"Rows {ca.StartRow}-{ca.EndRow}, Cols {ca.StartColumn}-{ca.EndColumn}");
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
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
