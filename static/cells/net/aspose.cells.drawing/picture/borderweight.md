##Picture.BorderWeight
Picture property. Gets or sets the weight of the border line of a picture in units of pt
## Picture.BorderWeight property
Gets or sets the weight of the border line of a picture in units of pt.
```csharp
public double BorderWeight { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyBorderWeightDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];
pic.BorderLineColor = Color.Red;
pic.BorderWeight = 3;
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
