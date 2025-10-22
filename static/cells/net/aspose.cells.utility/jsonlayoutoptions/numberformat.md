##JsonLayoutOptions.NumberFormat
JsonLayoutOptions property. Gets and sets the format of numeric value
## JsonLayoutOptions.NumberFormat property
Gets and sets the format of numeric value.
```csharp
public string NumberFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLayoutOptionsPropertyNumberFormatDemo
{
public static void Run()
{
// Create JSON data string
string jsonData = @"{
""Products"": [
{ ""ID"": 101, ""Price"": 19.95, ""Date"": ""2023-05-15"" },
{ ""ID"": 102, ""Price"": 29.99, ""Date"": ""2023-06-20"" }
]
}";
// Create JsonLayoutOptions with NumberFormat
JsonLayoutOptions layoutOptions = new JsonLayoutOptions
{
ArrayAsTable = true,
NumberFormat = "0.00",
DateFormat = "yyyy-MM-dd"
};
// Create workbook from JSON
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue(jsonData);
JsonUtility.ImportData(jsonData, workbook.Worksheets[0].Cells, 0, 0, layoutOptions);
// Save to Excel
workbook.Save("JsonNumberFormatDemo.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
