##Slicer.Placement
Slicer property. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet
## Slicer.Placement property
Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.
```csharp
public PlacementType Placement { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Drawing;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class SlicerPropertyPlacementDemo
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
worksheet.Cells["B3"].Value = 150;
worksheet.Cells["B4"].Value = 200;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Add a slicer for the pivot table
int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A6");
Slicer slicer = worksheet.Slicers[slicerIndex];
// Set slicer properties including Placement
slicer.Title = "Fruit Slicer";
slicer.Placement = PlacementType.MoveAndSize; // Demonstrate Placement property
slicer.HeightPixel = 200;
slicer.WidthPixel = 150;
// Save the workbook
workbook.Save("SlicerPlacementDemo.xlsx");
}
}
}
```
### See Also
* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
