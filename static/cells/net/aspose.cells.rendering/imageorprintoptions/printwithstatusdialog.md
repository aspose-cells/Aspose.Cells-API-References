##ImageOrPrintOptions.PrintWithStatusDialog
ImageOrPrintOptions property. If PrintWithStatusDialog  true  there will be a dialog that shows current print status. else no such dialog will show
## ImageOrPrintOptions.PrintWithStatusDialog property
If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.
```csharp
public bool PrintWithStatusDialog { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
{
public static void Run()
{
// Initialize a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Hello World!");
// Set image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.PrintWithStatusDialog = false; // Disable print status dialog
options.PageIndex = 0;
options.PageCount = 1;
// Create sheet render
SheetRender sheetRender = new SheetRender(worksheet, options);
// Print to PDF
sheetRender.ToImage(0, "output.png");
// Wait for file creation (simplified wait logic)
int attempts = 0;
while (!File.Exists("output.png") && attempts < 5)
{
Thread.Sleep(1000);
attempts++;
}
if (File.Exists("output.png"))
{
Console.WriteLine("Image file created successfully");
}
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
