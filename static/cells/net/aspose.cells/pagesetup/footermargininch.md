##PageSetup.FooterMarginInch
PageSetup property. Represents the distance from the bottom of the page to the footer in unit of inches
## PageSetup.FooterMarginInch property
Represents the distance from the bottom of the page to the footer, in unit of inches.
```csharp
public double FooterMarginInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyFooterMarginInchDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet and its PageSetup
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Set footer margin in inches
pageSetup.FooterMarginInch = 0.5;
// Set other margins for demonstration
pageSetup.HeaderMarginInch = 0.3;
pageSetup.TopMarginInch = 1.0;
pageSetup.BottomMarginInch = 1.0;
pageSetup.LeftMarginInch = 0.75;
pageSetup.RightMarginInch = 0.75;
// Save the workbook
workbook.Save("PageSetupMargins.xlsx");
// Print confirmation
Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
