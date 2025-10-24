##Slicer.Width
Slicer property. Returns or sets the width of the specified slicer in points
## Slicer.Width property
Returns or sets the width of the specified slicer, in points.
```csharp
[Obsolete("Use Shape.WidthPt property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double Width { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.WidthPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class SlicerPropertyWidthDemo
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
PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add a slicer
int slicerIndex = worksheet.Slicers.Add(pivotTable, 0, 0, "FruitSlicer");
Slicer slicer = worksheet.Slicers[slicerIndex];
// Correct way to add pivot connection to slicer
slicer.AddPivotConnection(pivotTable);
// Set slicer properties including Width
slicer.Caption = "Fruit Selection";
slicer.Width = 150; // Setting the width in points
slicer.Height = 200;
// Save the workbook
workbook.Save("SlicerWidthDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
