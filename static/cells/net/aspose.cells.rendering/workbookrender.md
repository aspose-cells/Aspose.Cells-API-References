##Class WorkbookRender
Aspose.Cells.Rendering.WorkbookRender class. Represents a Workbook render. The constructor of this class  must be used after modification of pagesetup cell style
## WorkbookRender class
Represents a Workbook render. The constructor of this class , must be used after modification of pagesetup, cell style.
```csharp
public class WorkbookRender
```
## Constructors
| Name | Description |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | The construct of WorkbookRender |
## Properties
| Name | Description |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Gets the total page count of workbook. |
## Methods
| Name | Description |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | Client can control page setting of printer when print each page using this function. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Releases resources created and used for rendering. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Get page size in inch of output image. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Render certain page to a Bitmap object. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Render whole workbook as Tiff Image to stream. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Render whole workbook as Tiff Image to a file. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Render certain page to a stream. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Render certain page to a file. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Render workbook to Printer |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Render workbook to Printer |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Render workbook to Printer |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Render workbook to Printer |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Render workbook to Printer |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingClassWorkbookRenderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and set page size
worksheet.Cells["A1"].PutValue("Workbook Render Demo");
worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;
// Create image options
ImageOrPrintOptions options = new ImageOrPrintOptions();
// Create workbook render and get page size
WorkbookRender render = new WorkbookRender(workbook, options);
float[] pageSize = render.GetPageSizeInch(0);
// Output the results
Console.WriteLine($"Page Width: {pageSize[0]} inches");
Console.WriteLine($"Page Height: {pageSize[1]} inches");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
