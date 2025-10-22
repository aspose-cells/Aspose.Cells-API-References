##LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate
LowCodeSaveOptionsProviderOfPlaceHolders property. The template for creating instance of save options in GetSaveOptions
## LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate property
The template for creating instance of save options in [`GetSaveOptions`](../getsaveoptions/).
```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```
### Remarks
If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;
using System;
public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySaveOptionsTemplateDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Sample Data";
// Initialize provider with path template containing placeholders
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/Sheet_{sheet}_Part_{part}.pdf");
// Display initial template state
Console.WriteLine($"Initial SaveOptionsTemplate: {(provider.SaveOptionsTemplate == null ? "Not set" : "Configured")}");
// Create and configure new save options template
provider.SaveOptionsTemplate = new LowCodePdfSaveOptions
{
PdfOptions = new PdfSaveOptions  // Fixed property name from PdfSaveOptions to PdfOptions
{
Compliance = PdfCompliance.PdfA1a,
ExportDocumentStructure = true
}
};
// Configure split parameters
provider.BuildPathWithSheetAlways = true;
provider.SplitPartPrefix = "Split_";
// Display configured PDF options
var pdfOptions = (LowCodePdfSaveOptions)provider.SaveOptionsTemplate;
Console.WriteLine($"Configured PDF Compliance: {pdfOptions.PdfOptions.Compliance}");  // Fixed property access
Console.WriteLine($"Document Structure Export: {pdfOptions.PdfOptions.ExportDocumentStructure}");  // Fixed property access
// Add page break to create split parts
worksheet.HorizontalPageBreaks.Add(0);
// Save using provider's configuration (actual split/save would occur here)
Console.WriteLine("Workbook prepared with SaveOptionsTemplate configuration");
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
