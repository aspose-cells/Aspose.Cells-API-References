##OoxmlSaveOptions.UpdateZoom
OoxmlSaveOptions property. Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled
## OoxmlSaveOptions.UpdateZoom property
Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled.
```csharp
public bool UpdateZoom { get; set; }
```
### Remarks
The default value is false for performance.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OoxmlSaveOptionsPropertyUpdateZoomDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set initial zoom level
worksheet.PageSetup.Zoom = 100;
// Create save options with UpdateZoom enabled
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
saveOptions.UpdateZoom = true;
// Save to memory stream
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, saveOptions);
// Reload the workbook to verify zoom was updated
stream.Position = 0;
Workbook reloadedWorkbook = new Workbook(stream);
Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
}
}
}
}
```
### See Also
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
