##PdfConverter.Process
PdfConverter method. Converts given template file to pdf
## Process(string, string) {#process_1}
Converts given template file to pdf.
```csharp
public static void Process(string templateFile, string resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be converted |
| resultFile | String | The resultant file, it must be pdf file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
using System.IO;
public class PdfConverterMethodProcessWithStringStringDemo
{
public static void Run()
{
// Create sample template file
CreateSampleTemplate("template.xlsx");
try
{
// Call Process method with (String, String) parameters directly on the type
PdfConverter.Process("template.xlsx", "output.pdf");
Console.WriteLine("Successfully converted template.xlsx to output.pdf");
Console.WriteLine($"PDF created at: {Path.GetFullPath("output.pdf")}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Process method: {ex.Message}");
}
}
private static void CreateSampleTemplate(string fileName)
{
using (Workbook workbook = new Workbook())
{
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("PDF Conversion Test");
worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
workbook.Save(fileName);
}
}
}
}
```
### See Also
* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}
Converts template file to pdf
```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class PdfConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
{
public static void Run()
{
// Create a sample input stream (Excel file in memory)
var workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue("Test Content");
MemoryStream template = new MemoryStream();
workbook.Save(template, SaveFormat.Xlsx);
template.Position = 0;
// Output directory
string outputDir = "Output/";
Directory.CreateDirectory(outputDir);
// Example 1: Convert to PDF
Aspose.Cells.LowCode.PdfConverter.Process(
new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
new Aspose.Cells.LowCode.LowCodePdfSaveOptions()
{
OutputFile = outputDir + "output.pdf",
PdfOptions = new PdfSaveOptions()
});
// Example 2: Convert to HTML
Aspose.Cells.LowCode.HtmlConverter.Process(
new Aspose.Cells.LowCode.LowCodeLoadOptions() { InputStream = template },
new Aspose.Cells.LowCode.LowCodeSaveOptions()
{
OutputFile = outputDir + "output.html"
});
Console.WriteLine("Conversion completed successfully.");
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [PdfConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
