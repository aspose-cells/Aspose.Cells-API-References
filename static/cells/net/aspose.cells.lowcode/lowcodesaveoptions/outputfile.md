##LowCodeSaveOptions.OutputFile
LowCodeSaveOptions property. Gets and sets the filewith path if needed for saving the generated data. When setting this property with value other than null or empty string OutputStream will be ignored
## LowCodeSaveOptions.OutputFile property
Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](../outputstream/) will be ignored.
```csharp
public string OutputFile { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class LowCodeSaveOptionsPropertyOutputFileDemo
{
public static void Run()
{
// Create a simple workbook with one worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World!");
// Save to different formats using OutputFile property
string outputDir = "Output/";
Directory.CreateDirectory(outputDir);
// Save as PDF
SaveWithOutputFile(workbook, SaveFormat.Pdf, "output.pdf");
// Save as JSON
SaveWithOutputFile(workbook, SaveFormat.Json, "output.json");
// Save as HTML
SaveWithOutputFile(workbook, SaveFormat.Html, "output.html");
// Save as CSV
SaveWithOutputFile(workbook, SaveFormat.Csv, "output.csv");
}
private static void SaveWithOutputFile(Workbook workbook, SaveFormat format, string fileName)
{
string outputPath = "Output/" + fileName;
switch (format)
{
case SaveFormat.Pdf:
PdfConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
new LowCodePdfSaveOptions { OutputFile = outputPath });
break;
case SaveFormat.Json:
JsonConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
new LowCodeSaveOptions { OutputFile = outputPath });
break;
case SaveFormat.Html:
HtmlConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
new LowCodeSaveOptions { OutputFile = outputPath });
break;
case SaveFormat.Csv:
TextConverter.Process(new LowCodeLoadOptions { InputStream = new MemoryStream() },
new LowCodeSaveOptions { OutputFile = outputPath });
break;
default:
throw new NotSupportedException("Format not supported: " + format);
}
Console.WriteLine($"File saved successfully to: {outputPath}");
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
