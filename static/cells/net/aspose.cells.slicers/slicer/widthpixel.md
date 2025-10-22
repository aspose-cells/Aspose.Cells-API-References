##Slicer.WidthPixel
Slicer property. Returns or sets the width of the specified slicer in pixels
## Slicer.WidthPixel property
Returns or sets the width of the specified slicer, in pixels.
```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerPropertyWidthPixelDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Banana");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(150);
sheet.Cells["B3"].PutValue(200);
int tableIndex = sheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = sheet.ListObjects[tableIndex];
int slicerIndex = sheet.Slicers.Add(table, 0, "A5");
Slicer slicer = sheet.Slicers[slicerIndex];
slicer.LeftPixel = 50;
slicer.TopPixel = 100;
slicer.WidthPixel = 120;
workbook.Save("SlicerWidthDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
