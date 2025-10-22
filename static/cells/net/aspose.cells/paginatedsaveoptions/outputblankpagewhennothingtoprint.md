##PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint
PaginatedSaveOptions property. Indicates whether to output a blank page when there is nothing to print
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property
Indicates whether to output a blank page when there is nothing to print.
```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```
### Remarks
Default is true.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and hide it (simulating nothing to print)
Worksheet worksheet = workbook.Worksheets[0];
worksheet.IsVisible = false;
// Set PDF save options with OutputBlankPageWhenNothingToPrint = false
PdfSaveOptions options = new PdfSaveOptions
{
OutputBlankPageWhenNothingToPrint = false
};
// Save to PDF - no blank page should be generated
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
workbook.Save(outputPath, options);
// Change the option to true
options.OutputBlankPageWhenNothingToPrint = true;
// Save again - a blank page should be generated
outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
workbook.Save(outputPath, options);
}
}
}
```
### See Also
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
