##Slicer.LockedPosition
Slicer property. Indicates whether the specified slicer can be moved or resized by using the user interface
## Slicer.LockedPosition property
Indicates whether the specified slicer can be moved or resized by using the user interface.
```csharp
public bool LockedPosition { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class SlicerPropertyLockedPositionDemo
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
// Create pivot table collection
PivotTableCollection pivotTables = worksheet.PivotTables;
// Create a pivot table
int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Create slicer collection
SlicerCollection slicers = worksheet.Slicers;
// Add a slicer for the pivot table
int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
Slicer slicer = slicers[slicerIndex];
// Set slicer properties
slicer.Caption = "Fruit Slicer";
slicer.NumberOfColumns = 2;
slicer.WidthPixel = 200;
slicer.HeightPixel = 150;
// Demonstrate LockedPosition property
slicer.LockedPosition = true; // Lock the slicer position
Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);
// Change the LockedPosition to false to allow movement
slicer.LockedPosition = false;
Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);
// Save the workbook
workbook.Save("SlicerLockedPositionDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
