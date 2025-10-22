##Picture.IsAutoSize
Picture property. True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated
## Picture.IsAutoSize property
True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.
```csharp
public bool IsAutoSize { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyIsAutoSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
Picture picture = worksheet.Pictures[pictureIndex];
// Demonstrate IsAutoSize property
Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
// Set IsAutoSize to true - picture will automatically resize to fit its content
picture.IsAutoSize = true;
Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
// Set IsAutoSize to false - picture will maintain its original dimensions
picture.IsAutoSize = false;
Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);
// Save the workbook
workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
