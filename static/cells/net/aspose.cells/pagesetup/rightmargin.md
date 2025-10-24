##PageSetup.RightMargin
PageSetup property. Represents the size of the right margin in unit of centimeters
## PageSetup.RightMargin property
Represents the size of the right margin, in unit of centimeters.
```csharp
public double RightMargin { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyRightMarginDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set different right margins and save to demonstrate the effect
worksheet.PageSetup.RightMargin = 0;
workbook.Save("RightMargin_0.xlsx");
worksheet.PageSetup.RightMargin = 1.0;
workbook.Save("RightMargin_1.xlsx");
worksheet.PageSetup.RightMargin = 2.5;
workbook.Save("RightMargin_2.5.xlsx");
// Print the current right margin value
Console.WriteLine("Current Right Margin: " + worksheet.PageSetup.RightMargin);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
