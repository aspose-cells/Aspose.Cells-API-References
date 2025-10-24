##Slicer.CaptionVisible
Slicer property. Returns or sets whether the header that displays the slicer Caption is visible the default value is true
## Slicer.CaptionVisible property
Returns or sets whether the header that displays the slicer Caption is visible the default value is true
```csharp
public bool CaptionVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class SlicerPropertyCaptionVisibleDemo
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
// Create a pivot table
int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = workbook.Worksheets[0].PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add a slicer
int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
Slicer slicer = worksheet.Slicers[slicerIndex];
// Set slicer properties including CaptionVisible
slicer.Caption = "Fruit Selection";
slicer.CaptionVisible = true; // Show the caption header
slicer.NumberOfColumns = 2;
slicer.StyleType = SlicerStyleType.SlicerStyleLight1;
// Save the workbook
workbook.Save("SlicerCaptionVisibleDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
