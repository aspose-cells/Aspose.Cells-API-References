##PivotTable.IsGridDropZones
PivotTable property. Indicates whether the PivotTable report displays classic pivottable layout. enables dragging fields in the grid
## PivotTable.IsGridDropZones property
Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)
```csharp
public bool IsGridDropZones { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyIsGridDropZonesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 300;
// Add pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Set IsGridDropZones property
pivotTable.IsGridDropZones = true;
Console.WriteLine("IsGridDropZones: " + pivotTable.IsGridDropZones);
// Save the workbook
workbook.Save("PivotTable_IsGridDropZones_Example.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
