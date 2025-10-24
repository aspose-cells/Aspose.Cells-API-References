##AutoFitterOptions.ForRendering
AutoFitterOptions property. Indicates whether fit for rendering purpose
## AutoFitterOptions.ForRendering property
Indicates whether fit for rendering purpose.
```csharp
public bool ForRendering { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyForRenderingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data with long text
worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
// Create AutoFitterOptions and set ForRendering to true
AutoFitterOptions options = new AutoFitterOptions();
options.ForRendering = true;
// Auto-fit the row with rendering considerations
worksheet.AutoFitRows(0, 0, options);
// Output the resulting row height in pixels
Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
}
}
}
```
### See Also
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
