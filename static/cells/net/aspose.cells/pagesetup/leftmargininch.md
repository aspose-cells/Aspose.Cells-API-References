##PageSetup.LeftMarginInch
PageSetup property. Represents the size of the left margin in unit of inches
## PageSetup.LeftMarginInch property
Represents the size of the left margin, in unit of inches.
```csharp
public double LeftMarginInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyLeftMarginInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup
PageSetup pageSetup = worksheet.PageSetup;
// Set left margin in inches (0.39 inches = ~1 cm)
pageSetup.LeftMarginInch = 0.39;
// Add some data to demonstrate the margin
worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");
// Save the workbook
workbook.Save("LeftMarginInchDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
