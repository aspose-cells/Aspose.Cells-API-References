##Enum PrintingPageType
Aspose.Cells.PrintingPageType enum. Indicates which pages will not be printed
## PrintingPageType enumeration
Indicates which pages will not be printed.
```csharp
public enum PrintingPageType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Prints all pages. |
| IgnoreBlank | `1` | Don't print the pages which the cells are blank. |
| IgnoreStyle | `2` | Don't print the pages which cells only contain styles. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class PrintingPageTypeDemo
{
public static void PrintingPageTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill some data in the worksheet
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["A2"].PutValue("World");
worksheet.Cells["A3"].PutValue("!");
// Create PdfSaveOptions
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Set the PrintingPageType to IgnoreBlank
pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
// Save the workbook to PDF with the specified options
workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
// Set the PrintingPageType to IgnoreStyle
pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
// Save the workbook to PDF with the specified options
workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
// Set the PrintingPageType to Default
pdfSaveOptions.PrintingPageType = PrintingPageType.Default;
// Save the workbook to PDF with the specified options
workbook.Save("output_default_page.pdf", pdfSaveOptions);
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
