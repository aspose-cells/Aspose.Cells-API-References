##Slicer.Title
Slicer property. Specifies the title of the current Slicer object
## Slicer.Title property
Specifies the title of the current Slicer object.
```csharp
public string Title { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class SlicerPropertyTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 20;
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:B4", "C1", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.CalculateData();
// Add slicer
SlicerCollection slicers = worksheet.Slicers;
int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
Slicer slicer = slicers[slicerIndex];
// Set slicer title
slicer.Title = "Fruit Selection Slicer";
// Save the workbook
workbook.Save("SlicerTitleDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
