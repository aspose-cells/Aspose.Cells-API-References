##Class JsonConverter
Aspose.Cells.LowCode.JsonConverter class. Converter for conversion between json data structure and other spreadsheet file formats
## JsonConverter class
Converter for conversion between json data structure and other spreadsheet file formats.
```csharp
public class JsonConverter
```
## Methods
| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converts between json data and other spreadsheet file formats. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | Converts given template file between json and other formats. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class LowCodeClassJsonConverterDemo
{
public static void Run()
{
string jsonFilePath = "data.json";
string excelFilePath = "res.xlsx";
try
{
// Convert JSON to Excel using Aspose.Cells.LowCode.JsonConverter
JsonConverter.Process(jsonFilePath, excelFilePath);
Console.WriteLine("Conversion completed successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Error during conversion: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
