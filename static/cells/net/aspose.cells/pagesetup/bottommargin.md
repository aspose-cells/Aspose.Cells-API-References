##PageSetup.BottomMargin
PageSetup property. Represents the size of the bottom margin in unit of centimeters
## PageSetup.BottomMargin property
Represents the size of the bottom margin, in unit of centimeters.
```csharp
public double BottomMargin { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PageSetupPropertyBottomMarginDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample data
worksheet.Cells["A1"].PutValue("Sample Text for Margin Demonstration");
// Configure page setup with BottomMargin
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.BottomMargin = 0.5; // 0.5 inch bottom margin
pageSetup.TopMargin = 1.0;    // 1 inch top margin
pageSetup.LeftMargin = 0.75;  // 0.75 inch left margin
pageSetup.RightMargin = 0.75; // 0.75 inch right margin
// Save to PDF to demonstrate margins
workbook.Save("PageMarginsDemo.pdf", SaveFormat.Pdf);
Console.WriteLine("Document with bottom margin of 0.5 inches created successfully.");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
