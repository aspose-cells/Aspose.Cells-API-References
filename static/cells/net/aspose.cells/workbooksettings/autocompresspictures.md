##WorkbookSettings.AutoCompressPictures
WorkbookSettings property. Specifies a boolean value that indicates the application automatically compressed pictures in the workbook
## WorkbookSettings.AutoCompressPictures property
Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.
```csharp
public bool AutoCompressPictures { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyAutoCompressPicturesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Enable AutoCompressPictures
workbook.Settings.AutoCompressPictures = true;
// Add a sample picture to demonstrate compression
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Pictures.Add(0, 0, "example.jpg");
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify the setting
Workbook loadedWorkbook = new Workbook("output.xlsx");
Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
