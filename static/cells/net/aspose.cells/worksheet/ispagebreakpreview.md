##Worksheet.IsPageBreakPreview
Worksheet property. Indicates whether the specified worksheet is shown in normal view or page break preview
## Worksheet.IsPageBreakPreview property
Indicates whether the specified worksheet is shown in normal view or page break preview.
```csharp
public bool IsPageBreakPreview { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIsPageBreakPreviewDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set the worksheet to Page Break Preview mode
worksheet.IsPageBreakPreview = true;
// Set zoom to 100% for demonstration
worksheet.Zoom = 100;
// Output the current settings
Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
Console.WriteLine("Zoom: " + worksheet.Zoom);
// Save the workbook
workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
