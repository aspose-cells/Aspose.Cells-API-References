##ImageOrPrintOptions.WarningCallback
ImageOrPrintOptions property. Gets or sets warning callback
## ImageOrPrintOptions.WarningCallback property
Gets or sets warning callback.
```csharp
public IWarningCallback WarningCallback { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class ImageOrPrintOptionsPropertyWarningCallbackDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add content that will generate a warning during rendering
worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
Style style = workbook.CreateStyle();
style.Font.Name = "NonExistentFont";
worksheet.Cells["A1"].SetStyle(style);
// Create ImageOrPrintOptions instance
ImageOrPrintOptions options = new ImageOrPrintOptions();
// Display initial WarningCallback value
Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);
// Create and assign custom warning callback
var warningCallback = new RenderingWarningCallback();
options.WarningCallback = warningCallback;
// Create SheetRender to demonstrate callback during rendering
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, "output_image.png");
// Check if warnings were captured
Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
}
}
// Custom callback implementation to handle rendering warnings
public class RenderingWarningCallback : IWarningCallback
{
public int WarningCount { get; private set; }
public void Warning(WarningInfo warningInfo)
{
// Handle font substitution warnings
if (warningInfo.WarningType == WarningType.FontSubstitution)
{
Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
WarningCount++;
}
}
}
}
```
### See Also
* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
