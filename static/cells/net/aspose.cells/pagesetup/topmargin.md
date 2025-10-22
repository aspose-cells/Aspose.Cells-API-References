##PageSetup.TopMargin
PageSetup property. Represents the size of the top margin in unit of centimeters
## PageSetup.TopMargin property
Represents the size of the top margin, in unit of centimeters.
```csharp
public double TopMargin { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PageSetupPropertyTopMarginDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data
sheet.Cells["A1"].PutValue("Top Margin Demonstration");
sheet.Cells["A2"].PutValue("This shows the effect of TopMargin property");
// Set page setup properties
PageSetup pageSetup = sheet.PageSetup;
pageSetup.TopMargin = 2.0; // 2 inches top margin
pageSetup.LeftMargin = 0.5;
pageSetup.RightMargin = 0.5;
pageSetup.BottomMargin = 1.0;
// Save to PDF to demonstrate the margins
string outputPath = "TopMarginDemo.pdf";
workbook.Save(outputPath, SaveFormat.Pdf);
Console.WriteLine("Document with top margin of 2 inches saved to: " + outputPath);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
