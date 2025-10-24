##Class WorkbookPrintingPreview
Aspose.Cells.Rendering.WorkbookPrintingPreview class. Workbook printing preview
## WorkbookPrintingPreview class
Workbook printing preview.
```csharp
public class WorkbookPrintingPreview
```
## Constructors
| Name | Description |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | The construct of WorkbookPrintingPreview |
## Properties
| Name | Description |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | Evaluate the total page count of this workbook |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class WorkbookPrintingPreviewDemo
{
public static void WorkbookPrintingPreviewExample()
{
// Load an existing workbook
Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");
// Create an instance of ImageOrPrintOptions
ImageOrPrintOptions options = new ImageOrPrintOptions();
// Create an instance of WorkbookPrintingPreview
WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);
// Evaluate the total page count of the workbook
int pageCount = workbookPrintingPreview.EvaluatedPageCount;
// Print the evaluated page count
Console.WriteLine("Total Page Count: " + pageCount);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
