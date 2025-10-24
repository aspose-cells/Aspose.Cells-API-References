##TextConverter.Process
TextConverter method. Converts given template file between text based files and other formats
## Process(string, string) {#process_1}
Converts given template file between text based files and other formats.
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
public class TextConverterMethodProcessWithStringStringDemo
{
public static void Run()
{
string inputFile = "input.csv";
string outputFile = "output.xlsx";
// Create sample CSV file
File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");
try
{
// Call the static Process method directly without instantiating TextConverter
TextConverter.Process(inputFile, outputFile);
Console.WriteLine($"Process method successfully converted {inputFile} to {outputFile}");
Console.WriteLine($"Converted file exists: {File.Exists(outputFile)}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Process method: {ex.Message}");
}
finally
{
// Cleanup temporary files
if (File.Exists(inputFile))
{
File.Delete(inputFile);
}
}
}
}
}
```
### See Also
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}
Converts file format between text based formats and other spreadsheet file formats
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
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class TextConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
{
public static void Run()
{
// Create a sample text file
string inputText = "Sample text content";
string inputPath = "input.txt";
File.WriteAllText(inputPath, inputText);
// Process the text file with LowCode options
using (FileStream inputStream = new FileStream(inputPath, FileMode.Open))
{
TextConverter.Process(
new LowCodeLoadOptions() { InputStream = inputStream },
new LowCodeSaveOptions()
{
OutputFile = "output.txt"
}
);
}
Console.WriteLine("Text processing completed successfully.");
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
