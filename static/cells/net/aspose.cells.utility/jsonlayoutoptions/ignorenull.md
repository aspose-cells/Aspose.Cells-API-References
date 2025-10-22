##JsonLayoutOptions.IgnoreNull
JsonLayoutOptions property. Indicates whether ignoring null value
## JsonLayoutOptions.IgnoreNull property
Indicates whether ignoring null value.
```csharp
public bool IgnoreNull { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLayoutOptionsPropertyIgnoreNullDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Sample JSON with null values
string json = @"{
""Name"": ""John"",
""Age"": 30,
""Address"": null,
""Salary"": 500.00
}";
// Configure JSON import options with IgnoreNull set to true
JsonLayoutOptions options = new JsonLayoutOptions();
options.IgnoreNull = true;
options.NumberFormat = "$0.00";
// Import JSON data to worksheet
JsonUtility.ImportData(json, cells, 0, 0, options);
// Verify the imported data (null Address should be ignored)
Console.WriteLine("Name: " + cells["A2"].StringValue);    // John
Console.WriteLine("Age: " + cells["B2"].IntValue);        // 30
Console.WriteLine("Address exists: " + (cells["C2"].Value != null)); // False
Console.WriteLine("Salary: " + cells["D2"].StringValue);  // $500.00
// Save the workbook
workbook.Save("JsonIgnoreNullDemo.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
