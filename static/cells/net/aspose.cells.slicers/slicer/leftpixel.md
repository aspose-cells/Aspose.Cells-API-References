##Slicer.LeftPixel
Slicer property. Returns or sets the horizontal offset of slicer shape from its left column in pixels
## Slicer.LeftPixel property
Returns or sets the horizontal offset of slicer shape from its left column, in pixels.
```csharp
[Obsolete("Use Shape.Left property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int LeftPixel { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerPropertyLeftPixelDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Fruit");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Orange");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(100);
sheet.Cells["B3"].PutValue(200);
int pivotIndex = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
int slicerIndex = sheet.Slicers.Add(pivotTable, "A10", 0);
Slicer slicer = sheet.Slicers[slicerIndex];
slicer.LeftPixel = 2;
workbook.Save("SlicerPropertyLeftPixelDemo_out.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
