##JsonSaveOptions.JsonSaveOptions
JsonSaveOptions constructor. Creates options for saving json file
## JsonSaveOptions constructor
Creates options for saving json file.
```csharp
public JsonSaveOptions()
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Sample data to export as JSON
workbook.Worksheets[0].Cells["A1"].PutValue("Name");
workbook.Worksheets[0].Cells["B1"].PutValue("Age");
workbook.Worksheets[0].Cells["A2"].PutValue("John");
workbook.Worksheets[0].Cells["B2"].PutValue(30);
// Initialize JsonSaveOptions using constructor
JsonSaveOptions options = new JsonSaveOptions();
// Set JSON export options
options.ExportNestedStructure = true;
options.SkipEmptyRows = true;
options.ValidateMergedAreas = true;
// Save workbook with JSON options
string outputPath = "output.json";
workbook.Save(outputPath, options);
Console.WriteLine("JSON file saved successfully with options.");
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
