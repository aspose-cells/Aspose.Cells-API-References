##WorkbookSettings.DefaultImageResolution
WorkbookSettings property. Gets and sets default resolution of image
## WorkbookSettings.DefaultImageResolution property
Gets and sets default resolution of image.
```csharp
public int DefaultImageResolution { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyDefaultImageResolutionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the default image resolution
workbook.Settings.DefaultImageResolution = 300;
// Add a worksheet and insert an image
Worksheet worksheet = workbook.Worksheets[0];
int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[imgIndex];
// Save the workbook
workbook.Save("output.xlsx");
// Verify the default image resolution
Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
