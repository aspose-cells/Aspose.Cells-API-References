##Picture.Copy
Picture method. Copy the picture
## Picture.Copy method
Copy the picture.
```csharp
public void Copy(Picture source, CopyOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | Picture | The source picture. |
| options | CopyOptions | The copy options. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PictureMethodCopyWithPictureCopyOptionsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Insert first picture (using a sample image path)
int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
Picture pic1 = worksheet.Pictures[imgIndex1];
// Insert second picture (using a sample image path)
int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
Picture pic2 = worksheet.Pictures[imgIndex2];
// Copy picture 1 to picture 2 with CopyOptions
CopyOptions options = new CopyOptions();
pic2.Copy(pic1, options);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
