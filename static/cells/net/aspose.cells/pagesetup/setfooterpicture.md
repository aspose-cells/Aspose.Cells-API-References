##PageSetup.SetFooterPicture
PageSetup method. Sets an image in the footer of a worksheet
## PageSetup.SetFooterPicture method
Sets an image in the footer of a worksheet.
```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerPicture | Byte[] | Image data. |
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
public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Load an image file into byte array
byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
try
{
// Call SetFooterPicture method with section index (0 for center, 1 for left, 2 for right) and image data
Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
// Set footer text to display along with the image
worksheet.PageSetup.SetFooter(0, "&G");
Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
// Save the workbook to see the footer image
workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
}
}
}
}
```
### See Also
* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
