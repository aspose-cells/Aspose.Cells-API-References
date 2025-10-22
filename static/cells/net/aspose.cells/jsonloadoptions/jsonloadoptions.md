##JsonLoadOptions.JsonLoadOptions
JsonLoadOptions constructor. Creates an options of loading the file
## JsonLoadOptions constructor
Creates an options of loading the file.
```csharp
public JsonLoadOptions()
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonLoadOptionsMethodCtorDemo
{
public static void Run()
{
// Source and output directories
string sourceDir = "SourceDir/";
string outputDir = "OutputDir/";
// Create JsonLoadOptions using constructor
JsonLoadOptions loadOptions = new JsonLoadOptions();
loadOptions.KeptSchema = true;
// Load JSON file with options
Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
// Save as Excel file
workbook.Save(outputDir + "example.xlsx");
// Save back to JSON with JsonSaveOptions
workbook.Save(outputDir + "example_output.json", new JsonSaveOptions()
{
ExportNestedStructure = true,
SkipEmptyRows = true
});
Console.WriteLine("JSON to Excel conversion completed successfully.");
}
}
}
```
### See Also
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
