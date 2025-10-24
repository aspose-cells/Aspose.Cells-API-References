##Picture.Data
Picture property. Gets the data of the picture
## Picture.Data property
Gets the data of the picture.
```csharp
public byte[] Data { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyDataDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Insert first picture
int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
Picture pic1 = worksheet.Pictures[imgIndex1];
// Insert second picture
int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
Picture pic2 = worksheet.Pictures[imgIndex2];
// Demonstrate Data property by copying image data
pic2.Data = pic1.Data;
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
