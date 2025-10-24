##PageSetup.TopMarginInch
PageSetup property. Represents the size of the top margin in unit of inches
## PageSetup.TopMarginInch property
Represents the size of the top margin, in unit of inches.
```csharp
public double TopMarginInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyTopMarginInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set top margin to 1.5 inches
sheet.PageSetup.TopMarginInch = 1.5;
// Get and print the top margin value
Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);
// Save the workbook
workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
