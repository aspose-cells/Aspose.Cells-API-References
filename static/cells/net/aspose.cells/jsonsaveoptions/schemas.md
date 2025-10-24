##JsonSaveOptions.Schemas
JsonSaveOptions property. The original json schema of each worksheet
## JsonSaveOptions.Schemas property
The original json schema of each worksheet.
```csharp
public string[] Schemas { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertySchemasDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Sample JSON data to import
string jsonData = @"{
""Products"": [
{
""ID"": 101,
""Name"": ""Product A"",
""Price"": 99.99
}
]
}";
// Import JSON data into worksheet
JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, new JsonLayoutOptions());
// Sample schema for validation
string schema = @"{
""$schema"": ""http://json-schema.org/draft-07/schema#"",
""type"": ""object"",
""properties"": {
""Products"": {
""type"": ""array"",
""items"": {
""type"": ""object"",
""properties"": {
""ID"": { ""type"": ""integer"" },
""Name"": { ""type"": ""string"" },
""Price"": { ""type"": ""number"" }
},
""required"": [""ID"", ""Name"", ""Price""]
}
}
},
""required"": [""Products""]
}";
// Configure JSON save options with schema
JsonSaveOptions saveOptions = new JsonSaveOptions();
saveOptions.Schemas = new string[] { schema };
saveOptions.ExportNestedStructure = true;
saveOptions.SkipEmptyRows = true;
// Save workbook with JSON options
string outputPath = "output_with_schema.json";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("Workbook saved with JSON schema validation.");
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
