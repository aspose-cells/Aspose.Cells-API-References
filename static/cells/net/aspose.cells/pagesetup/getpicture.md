##PageSetup.GetPicture
PageSetup method. Gets the Picture object of the header / footer
## GetPicture(bool, int) {#getpicture_1}
Gets the [`Picture`](../../../aspose.cells.drawing/picture/) object of the header / footer.
```csharp
public Picture GetPicture(bool isHeader, int section)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isHeader | Boolean | Indicates whether it is in the header or footer. |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
### Return Value
Returns [`Picture`](../../../aspose.cells.drawing/picture/) object. Returns null if there is no picture.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PageSetupMethodGetPictureWithBooleanInt32Demo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet's header
byte[] imageData = System.IO.File.ReadAllBytes("header.png");
worksheet.PageSetup.SetHeaderPicture(0, imageData);
// Get the picture from header and modify its brightness
Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
headerPicture.FormatPicture.Brightness = 50;
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetPicture(bool, bool, bool, int) {#getpicture}
Gets the [`Picture`](../../../aspose.cells.drawing/picture/) object of the header / footer.
```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isFirst | Boolean | Indicates whether getting the picture of first page header/footer. |
| isEven | Boolean | Indicates whether getting the picture of even page header/footer. |
| isHeader | Boolean | Indicates whether getting the picture of header/footer. |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
### Return Value
Returns [`Picture`](../../../aspose.cells.drawing/picture/) object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the PageSetup object
PageSetup pageSetup = worksheet.PageSetup;
// Set some header/footer properties to ensure we have pictures to retrieve
pageSetup.IsHFDiffFirst = true;
pageSetup.IsHFDiffOddEven = true;
try
{
// Call GetPicture method with parameters: isFirst, isEven, isHeader, section
// Checking first page header (section 0 - center header)
Picture picture = pageSetup.GetPicture(true, false, true, 0);
if (picture != null)
{
Console.WriteLine("Retrieved picture from first page header:");
Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
}
else
{
Console.WriteLine("No picture found in first page header");
}
// Save the workbook
workbook.Save("PageSetupGetPictureDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
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
