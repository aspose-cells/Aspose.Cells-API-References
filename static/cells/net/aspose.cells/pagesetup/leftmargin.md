##PageSetup.LeftMargin
PageSetup property. Represents the size of the left margin in unit of centimeters
## PageSetup.LeftMargin property
Represents the size of the left margin, in unit of centimeters.
```csharp
public double LeftMargin { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PageSetupPropertyLeftMarginDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set some sample data
sheet.Cells["A1"].PutValue("Left Margin Demonstration");
sheet.Cells["A2"].PutValue("This shows how to set page margins");
// Set left margin (in inches)
sheet.PageSetup.LeftMargin = 1.5;
// Print the left margin value to console
Console.WriteLine("Left Margin set to: " + sheet.PageSetup.LeftMargin + " inches");
// Save to PDF to demonstrate the margin
string outputPath = "LeftMarginDemo.pdf";
workbook.Save(outputPath, SaveFormat.Pdf);
Console.WriteLine("File saved with left margin: " + outputPath);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
