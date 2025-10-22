##Class LowCodePdfSaveOptions
Aspose.Cells.LowCode.LowCodePdfSaveOptions class. Options for saving pdf in low code way
## LowCodePdfSaveOptions class
Options for saving pdf in low code way.
```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](../lowcodesaveoptions/outputstream/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [`OutputFile`](../lowcodesaveoptions/outputfile/) will be ignored.(Inherited from [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | The options for saving Pdf file. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | The save format for the output. For converting to pdf, it can only be Pdf. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class LowCodeClassLowCodePdfSaveOptionsDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World!");
// Create PDF save options
PdfSaveOptions pdfOptions = new PdfSaveOptions();
pdfOptions.Compliance = PdfCompliance.PdfA1b;
// Create low-code PDF save options
LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
{
OutputFile = "output.pdf",
PdfOptions = pdfOptions
};
// Save using low-code options
workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);
Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
