##Slicer.HeightPixel
Slicer property. Returns or sets the height of the specified slicer in pixels
## Slicer.HeightPixel property
Returns or sets the height of the specified slicer, in pixels.
```csharp
[Obsolete("Use Shape.Height property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int HeightPixel { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class SlicerPropertyHeightPixelDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "A";
worksheet.Cells["A3"].Value = "B";
worksheet.Cells["A4"].Value = "C";
int tableIndex = worksheet.ListObjects.Add("A1", "A4", true);
ListObject table = worksheet.ListObjects[tableIndex];
int slicerIndex = worksheet.Slicers.Add(table, 0, "D1");
Slicer slicer = worksheet.Slicers[slicerIndex];
slicer.HeightPixel = 150;
workbook.Save("SlicerHeightDemo.xlsx");
}
}
}
```
### See Also
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
