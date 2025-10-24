##PageSetup.PrintDraft
PageSetup property. Represents if the sheet will be printed without graphics
## PageSetup.PrintDraft property
Represents if the sheet will be printed without graphics.
```csharp
public bool PrintDraft { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintDraftDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the PageSetup object
PageSetup pageSetup = worksheet.PageSetup;
// Set PrintDraft property to true
pageSetup.PrintDraft = true;
Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);
// Change PrintDraft property to false
pageSetup.PrintDraft = false;
Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);
// Save the workbook
workbook.Save("PageSetup_PrintDraft_Example.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
