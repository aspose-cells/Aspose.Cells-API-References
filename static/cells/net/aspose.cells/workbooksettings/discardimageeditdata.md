##WorkbookSettings.DiscardImageEditData
WorkbookSettings property. Indicates whether discarding editting image data
## WorkbookSettings.DiscardImageEditData property
Indicates whether discarding editting image data.
```csharp
public bool DiscardImageEditData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyDiscardImageEditDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add an image to the worksheet
int index = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[index];
// Set DiscardImageEditData to true (default is false)
workbook.Settings.DiscardImageEditData = true;
// Save the workbook
workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
// Verify the setting was applied
Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
