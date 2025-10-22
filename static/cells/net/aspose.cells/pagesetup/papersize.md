##PageSetup.PaperSize
PageSetup property. Represents the size of the paper
## PageSetup.PaperSize property
Represents the size of the paper.
```csharp
public PaperSizeType PaperSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPaperSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set the paper size to Envelope B6
sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;
// Print the current paper size
Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);
// Save the workbook
workbook.Save("PageSetup_PaperSizeDemo.xlsx");
}
}
}
```
### See Also
* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
