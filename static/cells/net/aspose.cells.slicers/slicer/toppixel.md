##Slicer.TopPixel
Slicer property. Returns or sets the vertical offset of slicer shape from its top row in pixels
## Slicer.TopPixel property
Returns or sets the vertical offset of slicer shape from its top row, in pixels.
```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerPropertyTopPixelDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data
sheet.Cells["A1"].Value = "Product";
sheet.Cells["A2"].Value = "Apple";
sheet.Cells["A3"].Value = "Orange";
sheet.Cells["A4"].Value = "Banana";
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["B2"].Value = 100;
sheet.Cells["B3"].Value = 200;
sheet.Cells["B4"].Value = 300;
// Create pivot table and get its index
int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.RefreshData();
pivotTable.CalculateData();
// Add slicer and get its index
int slicerIndex = sheet.Slicers.Add(pivotTable, "A6", 0);
Slicer slicer = sheet.Slicers[slicerIndex];
// Set TopPixel property
slicer.TopPixel = 6;
workbook.Save("SlicerTopPixelDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
