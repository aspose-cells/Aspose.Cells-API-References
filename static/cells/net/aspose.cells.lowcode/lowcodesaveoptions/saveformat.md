##LowCodeSaveOptions.SaveFormat
LowCodeSaveOptions property. Gets and sets the save format for the output. Generally for specific process in low code way only some specific formats are allowed. Please specify the correct format for corresponding process otherwise unexpected result or even exception may be caused
## LowCodeSaveOptions.SaveFormat property
Gets and sets the save format for the output. Generally, for specific process in low code way, only some specific formats are allowed. Please specify the correct format for corresponding process, otherwise unexpected result or even exception may be caused.
```csharp
public virtual SaveFormat SaveFormat { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsPropertySaveFormatDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(999.99);
// Initialize LowCodeSaveOptions with different formats
LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();
// Configure Excel save options
excelOptions.SaveFormat = SaveFormat.Xlsx;
excelOptions.OutputFile = "output_excel.xlsx";
// Configure PDF save options
pdfOptions.SaveFormat = SaveFormat.Pdf;
pdfOptions.OutputFile = "output_pdf.pdf";
// Demonstrate original format saving
Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);
// Demonstrate format change and re-save
Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);
Console.WriteLine("Files saved successfully with different formats.");
}
}
}
```
### See Also
* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
