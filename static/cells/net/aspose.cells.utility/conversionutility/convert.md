##ConversionUtility.Convert
ConversionUtility method. Converts Excel files to other formats
## Convert(string, string) {#convert_1}
Converts Excel files to other formats.
```csharp
public static void Convert(string source, string saveAs)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | String | The source file name. |
| saveAs | String | The file name of expected file. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class ConversionUtilityMethodConvertWithStringStringDemo
{
public static void Run()
{
// Initialize source and destination file paths
string sourcePath = "source.xlsx";
string destPath = "output.pdf";
// Convert Excel file to PDF
ConversionUtility.Convert(sourcePath, destPath);
Console.WriteLine("Conversion completed successfully.");
}
}
}
```
### See Also
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
## Convert(string, LoadOptions, string, SaveOptions) {#convert}
Converts Excel files to other formats.
```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs,
SaveOptions saveOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | String | The source file name. |
| loadOptions | LoadOptions | The options of loading the source file. |
| saveAs | String | The file name of expected file. |
| saveOptions | SaveOptions | The options of saving the file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Utility;
using System;
public class ConversionUtilityMethodConvertWithStringLoadOptionsStringSaveOptDemo
{
public static void Run()
{
// Source and destination file paths
string sourceFile = "input.csv";
string outputFile = "output.xlsx";
// Create sample CSV file for demonstration
System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");
try
{
// Create load options for CSV file
LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
// Create save options for XLSX file
SaveOptions saveOptions = new OoxmlSaveOptions();
// Convert CSV to XLSX with specified options
ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);
Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
// Verify the conversion by loading the output file
Workbook workbook = new Workbook(outputFile);
Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
}
catch (Exception ex)
{
Console.WriteLine($"Error during conversion: {ex.Message}");
}
finally
{
// Clean up temporary files
if (System.IO.File.Exists(sourceFile))
{
System.IO.File.Delete(sourceFile);
}
}
}
}
}
```
### See Also
* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
