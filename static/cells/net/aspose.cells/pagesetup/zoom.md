##PageSetup.Zoom
PageSetup property. Represents the scaling factor in percent. It should be between 10 and 400
## PageSetup.Zoom property
Represents the scaling factor in percent. It should be between 10 and 400.
```csharp
public int Zoom { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyZoomDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set zoom level to 150%
worksheet.PageSetup.Zoom = 150;
// Print current zoom level
Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
