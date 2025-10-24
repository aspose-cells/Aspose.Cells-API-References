##PageSetup.SetHeaderPicture
PageSetup method. Sets an image in the header of a worksheet
## PageSetup.SetHeaderPicture method
Sets an image in the header of a worksheet.
```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerPicture | Byte[] | Image data. |
### Return Value
Returns [`Picture`](../../../aspose.cells.drawing/picture/) object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Load an image file into byte array
byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
try
{
// Call SetHeaderPicture with section index (0 for center header) and image bytes
Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
// Set header script to display the image
worksheet.PageSetup.SetHeader(0, "&G");
Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
}
// Save the workbook
workbook.Save("SetHeaderPictureDemo.xlsx");
}
}
}
```
### See Also
* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
