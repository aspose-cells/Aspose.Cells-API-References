##Picture.IsLink
Picture property. Returns true if the picture is linked to a file
## Picture.IsLink property
Returns true if the picture is linked to a file.
```csharp
public bool IsLink { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyIsLinkDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a linked picture
int linkedPictureIndex = worksheet.Pictures.Add(0, 0, "https://example.com/image.jpg");
Picture linkedPicture = worksheet.Pictures[linkedPictureIndex];
// Add an embedded picture (using sample data)
byte[] embeddedImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample image data
using (MemoryStream stream = new MemoryStream(embeddedImageData))
{
int embeddedPictureIndex = worksheet.Pictures.Add(0, 5, stream);
Picture embeddedPicture = worksheet.Pictures[embeddedPictureIndex];
// Demonstrate IsLink property
Console.WriteLine("Linked picture IsLink: " + linkedPicture.IsLink);
Console.WriteLine("Embedded picture IsLink: " + embeddedPicture.IsLink);
// Show different behavior based on IsLink
Console.WriteLine("\nLinked picture data is null: " + (linkedPicture.Data == null));
Console.WriteLine("Embedded picture data length: " + embeddedPicture.Data.Length);
}
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
