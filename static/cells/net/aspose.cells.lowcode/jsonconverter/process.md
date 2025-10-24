##JsonConverter.Process
JsonConverter method. Converts given template file between json and other formats
## Process(string, string) {#process_1}
Converts given template file between json and other formats.
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
using Aspose.Cells.LowCode;
using System;
using System.IO;
public class JsonConverterMethodProcessWithStringStringDemo
{
public static void Run()
{
// Create sample JSON data and write to temporary file
string jsonData = "{\"employees\":[{\"name\":\"John\", \"department\":\"Sales\"}, {\"name\":\"Jane\", \"department\":\"Marketing\"}]}";
string templatePath = "template.json";
File.WriteAllText(templatePath, jsonData);
string resultPath = "output.xlsx";
try
{
// Process files directly using JsonConverter's static method
JsonConverter.Process(templatePath, resultPath);
Console.WriteLine($"Successfully converted JSON to spreadsheet. Output: {resultPath}");
}
catch (Exception ex)
{
Console.WriteLine($"Conversion error: {ex.Message}");
}
finally
{
// Clean up temporary JSON file
if (File.Exists(templatePath))
{
File.Delete(templatePath);
}
}
}
}
}
```
### See Also
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}
Converts between json data and other spreadsheet file formats.
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
public class JsonConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
{
public static void Run()
{
// Create sample JSON data
string jsonData = "{\"name\":\"John\", \"age\":30, \"city\":\"New York\"}";
// Create a memory stream with the JSON data
using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(jsonData)))
{
// Process the JSON data with LowCode options
JsonConverter.Process(
new LowCodeLoadOptions() { InputStream = stream },
new LowCodeSaveOptions()
{
OutputFile = "output.json"
});
}
Console.WriteLine("JSON processing completed successfully.");
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [JsonConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
