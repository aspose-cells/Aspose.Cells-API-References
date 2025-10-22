##JsonLayoutOptions.IgnoreTitle
JsonLayoutOptions property. Ingores titles of attributes
## JsonLayoutOptions.IgnoreTitle property
Ingores titles of attributes
```csharp
public bool IgnoreTitle { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLayoutOptionsPropertyIgnoreTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample JSON data
string jsonInput = @"{
""Products"": [
{
""Name"": ""Product1"",
""Price"": 100,
""Date"": ""2023-01-15""
},
{
""Name"": ""Product2"",
""Price"": 200,
""Date"": ""2023-02-20""
}
]
}";
// Set JsonLayoutOptions with IgnoreTitle = true
JsonLayoutOptions options = new JsonLayoutOptions();
options.IgnoreTitle = true;  // This will skip the title row in output
options.ArrayAsTable = true;
options.DateFormat = "yyyy/MM/dd";
// Import JSON data
JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);
// Save the workbook
workbook.Save("output_ignore_title.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
