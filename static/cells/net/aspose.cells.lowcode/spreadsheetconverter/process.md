##SpreadsheetConverter.Process
SpreadsheetConverter method. Converts given template file between spreadsheet file formats
## Process(string, string) {#process_1}
Converts given template file between spreadsheet file formats.
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
public class SpreadsheetConverterMethodProcessWithStringStringDemo
{
public static void Run()
{
SpreadsheetConverter.Process("file1.xlsx", "SpreadsheetConverterMethodProcessWithStringStringDemo.xlsb");
}
}
}
```
### See Also
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}
Converts between different spreadsheet file formats.
```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options for input and loading |
| saveOptions | LowCodeSaveOptions | Options for output and saving |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
{
public static void Run()
{
// Create load options with input file
LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
loadOptions.InputFile = "file1.xlsx";
// Create save options with output file
LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
saveOptions.OutputFile = "SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo.xlsx";
// Execute conversion
SpreadsheetConverter.Process(loadOptions, saveOptions);
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
