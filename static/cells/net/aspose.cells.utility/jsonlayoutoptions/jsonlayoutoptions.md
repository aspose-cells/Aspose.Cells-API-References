##JsonLayoutOptions.JsonLayoutOptions
JsonLayoutOptions constructor. Constructor of loading JSON layout options
## JsonLayoutOptions constructor
Constructor of loading JSON layout options.
```csharp
public JsonLayoutOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLayoutOptionsMethodCtorDemo
{
public static void Run()
{
// Create sample JSON data
string json = @"{
""Name"": ""John"",
""Age"": 30,
""Address"": {
""Street"": ""123 Main St"",
""City"": ""New York""
}
}";
// Create a new workbook
Workbook workbook = new Workbook();
// Initialize JsonLayoutOptions using constructor
JsonLayoutOptions options = new JsonLayoutOptions();
// Set options
options.ArrayAsTable = true;
options.IgnoreArrayTitle = false;
options.IgnoreObjectTitle = false;
// Import JSON data to worksheet
JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options);
// Save the workbook
workbook.Save("JsonImportDemo.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
