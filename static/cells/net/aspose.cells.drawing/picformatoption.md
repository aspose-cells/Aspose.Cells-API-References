##Class PicFormatOption
Aspose.Cells.Drawing.PicFormatOption class. Represents picture format option
## PicFormatOption class
Represents picture format option
```csharp
public class PicFormatOption
```
## Constructors
| Name | Description |
| --- | --- |
| [PicFormatOption](picformatoption/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | Gets or sets the bottom offset for stretching picture. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | Gets or sets the left offset for stretching picture. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | Gets or sets the right offset for stretching picture. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | Gets or sets how many the picture stack and scale with. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | Gets or sets the top offset for stretching picture. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | Gets or sets the picture fill type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.IO;
public class DrawingClassPicFormatOptionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set picture fill
Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
// FillType property removed from MsoFillFormat access
shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");
// Configure picture format options
PicFormatOption picFormat = new PicFormatOption
{
Type = FillPictureType.Stretch,
Left = 0.15,
Right = 0.15,
Top = 0.15,
Bottom = 0.15,
Scale = 0.8
};
// Add second shape with tiled image
Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
// FillType property removed from MsoFillFormat access
tiledShape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");
PicFormatOption tileFormat = new PicFormatOption
{
Type = FillPictureType.Stack,
Scale = 1.5
};
workbook.Save("PicFormatOptionDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
