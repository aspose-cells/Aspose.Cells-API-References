##PageSetup.FooterMargin
PageSetup property. Represents the distance from the bottom of the page to the footer in unit of centimeters
## PageSetup.FooterMargin property
Represents the distance from the bottom of the page to the footer, in unit of centimeters.
```csharp
public double FooterMargin { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyFooterMarginDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup
PageSetup pageSetup = worksheet.PageSetup;
// Set footer margin in centimeters
pageSetup.FooterMargin = 1.5;
// Add some content to see the effect
worksheet.Cells["A1"].PutValue("Footer Margin Demo");
worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");
// Set footer text to make margin visible
pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");
// Save the workbook
workbook.Save("FooterMarginDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
