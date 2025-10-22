##PivotTable.PrintDrill
PivotTable property. Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable
## PivotTable.PrintDrill property
Specifies a boolean value that indicates whether drill indicators should be printed. print expand/collapse buttons when displayed on pivottable.
```csharp
public bool PrintDrill { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyPrintDrillDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
var cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "Bikes";
cells["B2"].Value = 1000;
cells["A3"].Value = "Cars";
cells["B3"].Value = 2000;
cells["A4"].Value = "Bikes";
cells["B4"].Value = 1500;
cells["A5"].Value = "Cars";
cells["B5"].Value = 2500;
// Add a pivot table
int index = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Demonstrate PrintDrill property
pivotTable.PrintDrill = false; // Disable printing drill indicators
pivotTable.ShowDrill = true;   // Show drill indicators on screen
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTablePrintDrillDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
