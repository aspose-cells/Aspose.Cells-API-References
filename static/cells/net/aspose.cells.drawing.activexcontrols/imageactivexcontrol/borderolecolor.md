##ImageActiveXControl.BorderOleColor
ImageActiveXControl property. Gets and sets the ole color of the background
## ImageActiveXControl.BorderOleColor property
Gets and sets the ole color of the background.
```csharp
public int BorderOleColor { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageActiveXControlPropertyBorderOleColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 5, 0, 1, 1, 100, 100);
Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;
imageControl.BorderOleColor = 0x0000FF; // Blue border
imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
// Create a simple image in memory if demo file doesn't exist
byte[] imageData;
if (!File.Exists("demo.jpg"))
{
// Alternative image creation without System.Drawing
imageData = CreateSampleImage(100, 100);
}
else
{
imageData = File.ReadAllBytes("demo.jpg");
}
imageControl.Picture = imageData;
workbook.Save("ImageActiveXControlBorderColorDemo.xlsx");
Console.WriteLine($"Border color set to: {imageControl.BorderOleColor:X6}");
}
private static byte[] CreateSampleImage(int width, int height)
{
// Create a simple grayscale image without System.Drawing
byte[] pixels = new byte[width * height * 3]; // RGB
for (int i = 0; i < pixels.Length; i++)
{
pixels[i] = 200; // Light gray color
}
return pixels;
}
}
}
```
### See Also
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
