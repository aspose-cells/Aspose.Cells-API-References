##JsonLayoutOptions.KeptSchema
JsonLayoutOptions property. Indicates whether keeping schema of this json
## JsonLayoutOptions.KeptSchema property
Indicates whether keeping schema of this json.
```csharp
public bool KeptSchema { get; set; }
```
### Remarks
Sometimes we will save the file to JSON after loading JSON file.
### Examples
```csharp
using System;
using System.IO;
using System.Text.Json;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLayoutOptionsPropertyKeptSchemaDemo
{
public class Data
{
public string RootProperty { get; set; }
public Payload Payload { get; set; }
}
public class Payload
{
public ArrayData[] Array { get; set; }
public string PayloadProperty { get; set; }
public PayloadStruct PayloadStruct { get; set; }
}
public class ArrayData
{
public string ArrayProperty { get; set; }
}
public struct PayloadStruct
{
public string PayloadProperty1 { get; set; }
public string PayloadProperty2 { get; set; }
}
public static void Run()
{
// Create sample data
var data = new Data()
{
RootProperty = "RootValue",
Payload = new Payload()
{
Array = new[]
{
new ArrayData() { ArrayProperty = "item1" },
new ArrayData() { ArrayProperty = "item2" }
},
PayloadProperty = "PayloadValue",
PayloadStruct = new PayloadStruct()
{
PayloadProperty1 = "struct1",
PayloadProperty2 = "struct2"
}
}
};
// Serialize to JSON using System.Text.Json
string json = JsonSerializer.Serialize(new[] { data });
// Create workbook and import JSON
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
layoutOptions.KeptSchema = true; // Demonstrate KeptSchema usage
JsonUtility.ImportData(json, worksheet.Cells, 0, 0, layoutOptions);
// Save and output results
string outputPath = "output/";
Directory.CreateDirectory(outputPath);
workbook.Save(outputPath + "KeptSchemaDemo.xlsx", SaveFormat.Xlsx);
workbook.Save(outputPath + "KeptSchemaDemo.json", new JsonSaveOptions()
{
ExportNestedStructure = true
});
Console.WriteLine("Files saved successfully. Check output directory.");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
