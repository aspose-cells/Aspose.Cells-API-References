##Picture.OriginalHeight
Picture property. Gets the original height of the picture
## Picture.OriginalHeight property
Gets the original height of the picture.
```csharp
public int OriginalHeight { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyOriginalHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
Picture pic = worksheet.Pictures[imgIndex];
// Get and display the original height of the picture
int originalHeight = pic.OriginalHeight;
Console.WriteLine("Original height of the picture: " + originalHeight + " pixels");
// Save the workbook
workbook.Save("result.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
