##PageSetup.RightMarginInch
PageSetup property. Represents the size of the right margin in unit of inches
## PageSetup.RightMarginInch property
Represents the size of the right margin, in unit of inches.
```csharp
public double RightMarginInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyRightMarginInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup and set RightMarginInch
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.RightMarginInch = 0.75; // Set right margin to 0.75 inches
// Add some sample data to see the effect
worksheet.Cells["A1"].PutValue("Right Margin Demo");
for (int i = 1; i <= 10; i++)
{
worksheet.Cells["B" + i].PutValue("Sample Data " + i);
}
// Save the workbook
workbook.Save("RightMarginInchDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
