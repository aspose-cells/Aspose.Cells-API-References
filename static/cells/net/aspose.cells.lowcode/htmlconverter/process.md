##HtmlConverter.Process
HtmlConverter method. Converts given template file between html and other formats
## Process(string, string) {#process_1}
Converts given template file between html and other formats.
```csharp
public static void Process(string templateFile, string resultFile)
```
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | String | The template file to be converted |
| resultFile | String | The resultant file |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
using System.IO;
public class HtmlConverterMethodProcessWithStringStringDemo
{
public static void Run()
{
// Create temporary HTML file for conversion
string templateFile = CreateSampleHtmlFile();
string resultFile = "HtmlConversionResult.xlsx";
try
{
// Process the files directly using HtmlConverter
HtmlConverter.Process(templateFile, resultFile);
Console.WriteLine($"Successfully converted '{templateFile}' to '{resultFile}'");
}
catch (Exception ex)
{
Console.WriteLine($"Error during conversion: {ex.Message}");
}
finally
{
// Clean up temporary file
if (File.Exists(templateFile))
{
File.Delete(templateFile);
}
}
}
private static string CreateSampleHtmlFile()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample HTML Conversion");
string tempFile = Path.GetTempFileName() + ".html";
workbook.Save(tempFile, SaveFormat.Html);
return tempFile;
}
}
}
```
### See Also
* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}
Converts file between html and other spreadsheet file formats.
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
public class HtmlConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
{
public static void Run()
{
// Create a simple HTML template in memory
string htmlContent = "<html><body><h1>Test Document</h1><p>This is a test HTML document.</p></body></html>";
using (MemoryStream template = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(htmlContent)))
{
// Convert to PDF using LowCode options
HtmlConverter.Process(
new LowCodeLoadOptions() { InputStream = template },
new LowCodeSaveOptions()
{
OutputFile = "output.pdf",
SaveFormat = SaveFormat.Pdf
});
// Reset stream position for next conversion
template.Position = 0;
// Convert to HTML using LowCode options
HtmlConverter.Process(
new LowCodeLoadOptions() { InputStream = template },
new LowCodeSaveOptions()
{
OutputFile = "output.html",
SaveFormat = SaveFormat.Html
});
}
Console.WriteLine("Conversions completed successfully.");
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [HtmlConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
