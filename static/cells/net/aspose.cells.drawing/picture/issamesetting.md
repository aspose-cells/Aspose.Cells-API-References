##Picture.IsSameSetting
Picture method. Returns whether the shape is same
## Picture.IsSameSetting method
Returns whether the shape is same.
```csharp
public override bool IsSameSetting(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PictureMethodIsSameSettingWithObjectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Insert first picture (using a sample image path)
int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
Picture pic1 = worksheet.Pictures[imgIndex1];
// Insert second picture (using a different sample image path)
int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
Picture pic2 = worksheet.Pictures[imgIndex2];
// Compare picture with itself
if (pic1.IsSameSetting(pic1))
{
Console.WriteLine("pic1 and pic1 are the same");
}
// Compare different pictures
if (!pic1.IsSameSetting(pic2))
{
Console.WriteLine("pic1 and pic2 are different");
}
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
