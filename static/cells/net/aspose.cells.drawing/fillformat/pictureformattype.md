##FillFormat.PictureFormatType
FillFormat property. Gets and sets the picture format type
## FillFormat.PictureFormatType property
Gets and sets the picture format type.
```csharp
public FillPictureType PictureFormatType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyPictureFormatTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate picture fill
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);
// Set picture fill properties
shape.Fill.Type = FillType.Texture;
shape.Fill.Texture = TextureType.BlueTissuePaper;
shape.Fill.PictureFormatType = FillPictureType.Stretch;
// Save the workbook
workbook.Save("FillFormatPictureTypeDemo.xlsx");
// Load the saved workbook to verify properties
Workbook verifyWorkbook = new Workbook("FillFormatPictureTypeDemo.xlsx");
Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
// Output the PictureFormatType to demonstrate its usage
Console.WriteLine("PictureFormatType: " + verifyShape.Fill.PictureFormatType);
}
}
}
```
### See Also
* enum [FillPictureType](../../fillpicturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
