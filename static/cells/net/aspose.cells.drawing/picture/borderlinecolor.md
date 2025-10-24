##Picture.BorderLineColor
Picture property. Represents the Color of the border line of a picture
## Picture.BorderLineColor property
Represents the Color of the border line of a picture.
```csharp
public Color BorderLineColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyBorderLineColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
Picture pic = worksheet.Pictures[imgIndex];
pic.BorderLineColor = Color.Red;
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
