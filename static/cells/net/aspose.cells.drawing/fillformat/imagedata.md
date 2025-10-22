##FillFormat.ImageData
FillFormat property. Gets and sets the picture image data
## FillFormat.ImageData property
Gets and sets the picture image data.
```csharp
public byte[] ImageData { get; set; }
```
### Remarks
If the fill format is not custom texture format, returns null.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FillFormatPropertyImageDataDemo
{
public static void Run()
{
// Create workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample image to worksheet
string imagePath = "example.png";
worksheet.Pictures.Add(0, 0, imagePath);
// Create comment and set image data
var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
byte[] imageData = File.ReadAllBytes(imagePath);
comment.CommentShape.Fill.ImageData = imageData;
// Save workbook
workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
