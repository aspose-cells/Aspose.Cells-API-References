##Picture.SourceFullName
Picture property. Gets or sets the path and name of the source file for the linked image
## Picture.SourceFullName property
Gets or sets the path and name of the source file for the linked image.
```csharp
public string SourceFullName { get; set; }
```
### Remarks
The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertySourceFullNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a linked picture to the worksheet
string imagePath = "example.png";
Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);
// Demonstrate SourceFullName property
Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
Console.WriteLine("Is linked picture: " + picture.IsLink);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
