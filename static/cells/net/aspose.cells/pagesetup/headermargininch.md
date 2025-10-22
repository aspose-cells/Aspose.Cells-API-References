##PageSetup.HeaderMarginInch
PageSetup property. Represents the distance from the top of the page to the header in unit of inches
## PageSetup.HeaderMarginInch property
Represents the distance from the top of the page to the header, in unit of inches.
```csharp
public double HeaderMarginInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyHeaderMarginInchDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet and its PageSetup
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Set header margin in inches
pageSetup.HeaderMarginInch = 0.5;
// Set other margins for demonstration
pageSetup.FooterMarginInch = 0.25;
pageSetup.TopMarginInch = 1.0;
pageSetup.BottomMarginInch = 1.0;
pageSetup.LeftMarginInch = 0.75;
pageSetup.RightMarginInch = 0.75;
// Save the workbook
workbook.Save("PageSetupMargins.xlsx");
// Display the header margin value
Console.WriteLine("Header Margin (inches): " + pageSetup.HeaderMarginInch);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
