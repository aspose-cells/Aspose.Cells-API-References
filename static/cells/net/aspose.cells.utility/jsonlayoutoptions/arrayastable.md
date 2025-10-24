##JsonLayoutOptions.ArrayAsTable
JsonLayoutOptions property. Processes Array as table
## JsonLayoutOptions.ArrayAsTable property
Processes Array as table.
```csharp
public bool ArrayAsTable { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLayoutOptionsPropertyArrayAsTableDemo
{
public static void Run()
{
// Create a workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create JSON layout options and set ArrayAsTable to true
JsonLayoutOptions options = new JsonLayoutOptions();
options.ArrayAsTable = true;
options.IgnoreTitle = true;
// Sample JSON data (simplified for demonstration)
string jsonData = @"{
""products"": [
{""id"":1, ""name"":""Laptop"", ""price"":999.99},
{""id"":2, ""name"":""Phone"", ""price"":599.99}
]
}";
// Import JSON data to worksheet
JsonUtility.ImportData(jsonData, sheet.Cells, 0, 0, options);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
