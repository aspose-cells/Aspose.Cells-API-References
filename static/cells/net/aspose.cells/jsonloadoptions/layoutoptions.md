##JsonLoadOptions.LayoutOptions
JsonLoadOptions property. The options of import json
## JsonLoadOptions.LayoutOptions property
The options of import json.
```csharp
public JsonLayoutOptions LayoutOptions { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLoadOptionsPropertyLayoutOptionsDemo
{
public static void Run()
{
// Create JSON load options with LayoutOptions
JsonLoadOptions options = new JsonLoadOptions
{
LayoutOptions = new JsonLayoutOptions
{
ArrayAsTable = true,
IgnoreNull = false,
ConvertNumericOrDate = true,
NumberFormat = "0.00",
DateFormat = "yyyy-MM-dd"
}
};
// Create a new workbook with JSON data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample JSON data
string json = @"{
""Products"": [
{ ""ID"": 1, ""Name"": ""Product A"", ""Price"": 19.99, ""Date"": ""2023-05-15"" },
{ ""ID"": 2, ""Name"": ""Product B"", ""Price"": 29.99, ""Date"": ""2023-06-20"" }
]
}";
// Import JSON to worksheet
JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options.LayoutOptions);
// Save the workbook
workbook.Save("JsonWithLayoutOptions.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../../../aspose.cells.utility/jsonlayoutoptions/)
* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
