##PageSetup.HeaderMargin
PageSetup property. Represents the distance from the top of the page to the header in unit of centimeters
## PageSetup.HeaderMargin property
Represents the distance from the top of the page to the header, in unit of centimeters.
```csharp
public double HeaderMargin { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyHeaderMarginDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup
PageSetup pageSetup = worksheet.PageSetup;
// Set header margin in centimeters
pageSetup.HeaderMargin = 1.5;
// Verify the header margin was set
Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");
// Save the workbook
workbook.Save("HeaderMarginDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
