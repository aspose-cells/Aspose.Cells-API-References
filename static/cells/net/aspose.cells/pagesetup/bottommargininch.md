##PageSetup.BottomMarginInch
PageSetup property. Represents the size of the bottom margin in unit of inches
## PageSetup.BottomMarginInch property
Represents the size of the bottom margin, in unit of inches.
```csharp
public double BottomMarginInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyBottomMarginInchDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet's PageSetup
PageSetup setup = workbook.Worksheets[0].PageSetup;
// Set various margins in inches
setup.HeaderMarginInch = 0.1;
setup.FooterMarginInch = 0.2;
setup.TopMarginInch = 0.3;
setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
setup.LeftMarginInch = 0.5;
setup.RightMarginInch = 0.6;
// Save the workbook
workbook.Save("PageMarginsDemo.xlsx");
// Display confirmation
Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
