##PageSetup.CustomPaperSize
PageSetup method. Sets the custom paper size in unit of inches
## PageSetup.CustomPaperSize method
Sets the custom paper size, in unit of inches.
```csharp
public void CustomPaperSize(double width, double height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| width | Double | The width of the paper. |
| height | Double | The height of the paper. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set custom paper size (width: 1.5 inches, height: 1.5 inches)
worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
// Save the workbook to demonstrate the effect
workbook.Save("CustomPaperSizeDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
