##PageSetup.PrintQuality
PageSetup property. Represents the print quality
## PageSetup.PrintQuality property
Represents the print quality.
```csharp
public int PrintQuality { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintQualityDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set print quality to 144 dpi
worksheet.PageSetup.PrintQuality = 144;
// Print the current print quality setting
Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
// Save the workbook
workbook.Save("PrintQualityDemo.xls");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
