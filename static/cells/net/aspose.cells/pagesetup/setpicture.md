##PageSetup.SetPicture
PageSetup method. Sets an image in the header/footer of a worksheet
## PageSetup.SetPicture method
Sets an image in the header/footer of a worksheet.
```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | Boolean | Indicates whether setting the picture of first page header/footer. |
| isEven | Boolean | Indicates whether setting the picture of even page header/footer. |
| isHeader | Boolean | Indicates whether setting the picture of header/footer. |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| imageData | Byte[] | Image data. |
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
public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Load an image file into byte array
byte[] imageData = File.ReadAllBytes("example.jpg");
try
{
// Call SetPicture method to set header picture
// Parameters: isFirstPage, isEvenPage, isHeader, section, imageData
Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);
// Set header text
pageSetup.SetHeader(1, "&G");
Console.WriteLine("SetPicture method executed successfully. Header image set.");
// Save the workbook
workbook.Save("PageSetupSetPictureDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
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
