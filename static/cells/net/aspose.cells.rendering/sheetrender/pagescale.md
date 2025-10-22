##SheetRender.PageScale
SheetRender property. Gets calculated page scale of the sheet. Returns the set scale if Zoom is set. Otherwise returns the calculated scale according to FitToPagesWide and FitToPagesTall
## SheetRender.PageScale property
Gets calculated page scale of the sheet. Returns the set scale if [`Zoom`](../../../aspose.cells/pagesetup/zoom/) is set. Otherwise, returns the calculated scale according to [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) and [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/).
```csharp
public double PageScale { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class SheetRenderPropertyPageScaleDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data to cells
for (int i = 0; i < 10; i++)
{
sheet.Cells[i, 0].PutValue($"Item {i + 1}");
sheet.Cells[i, 1].PutValue((i + 1) * 10);
}
// Create image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
// Create sheet render
SheetRender sheetRender = new SheetRender(sheet, options);
// Get and display the calculated page scale
double pageScale = sheetRender.PageScale;
Console.WriteLine($"Calculated Page Scale: {pageScale}");
}
}
}
```
### See Also
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
