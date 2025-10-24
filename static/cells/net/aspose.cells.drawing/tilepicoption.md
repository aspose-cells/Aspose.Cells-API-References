##Class TilePicOption
Aspose.Cells.Drawing.TilePicOption class. Represents tile picture as texture
## TilePicOption class
Represents tile picture as texture.
```csharp
public class TilePicOption
```
## Constructors
| Name | Description |
| --- | --- |
| [TilePicOption](tilepicoption/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Gets or sets the alignment for tiling. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Gets or sets the mirror type for tiling. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Gets or sets the X offset for tiling picture. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Gets or sets the Y offset for tiling picture. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Gets or sets the X scale for tiling picture. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Gets or sets the Y scale for tiling picture. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassTilePicOptionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart for demonstration
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set fill type to texture
chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;
// Load sample image (replace with actual path)
byte[] imageData = File.ReadAllBytes("sample.png");
chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
// Create and configure TilePicOption
TilePicOption tileOptions = new TilePicOption();
tileOptions.ScaleX = 50;
tileOptions.ScaleY = 50;
chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;
// Save the workbook
workbook.Save("TilePicOptionDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
