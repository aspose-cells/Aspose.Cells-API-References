##MsoFillFormat.ImageData
MsoFillFormat property. Gets and sets the Texture and Picture fill data
## MsoFillFormat.ImageData property
Gets and sets the Texture and Picture fill data.
```csharp
public byte[] ImageData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoFillFormatPropertyImageDataDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Shape shape = sheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
MsoFillFormat fillFormat = shape.FillFormat;
byte[] imageData = new byte[]
{
0x42, 0x4D, 0x3A, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x18, 0x00,
0x00, 0x00, 0x00, 0x00, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0xFF, 0x00
};
fillFormat.ImageData = imageData;
workbook.Save("output.ods");
Workbook reloadedWorkbook = new Workbook("output.ods");
Console.WriteLine(reloadedWorkbook.Worksheets[0].Shapes[0].FillFormat.ImageData != null
? "ImageData exists"
: "ImageData missing");
}
}
}
```
### See Also
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
