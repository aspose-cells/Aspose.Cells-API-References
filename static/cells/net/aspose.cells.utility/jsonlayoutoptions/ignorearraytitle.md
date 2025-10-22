##JsonLayoutOptions.IgnoreArrayTitle
JsonLayoutOptions property. Indicates whether ignore title if array is a property of object
## JsonLayoutOptions.IgnoreArrayTitle property
Indicates whether ignore title if array is a property of object.
```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreArrayTitle { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use JsonLayoutOptions.IgnoreTitle property instead. This property will be removed 6 months later since February 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Utility;
using System;
public class JsonLayoutOptionsPropertyIgnoreArrayTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample JSON data with array titles
string json = @"{
""Employees"": [
{ ""Name"": ""John"", ""Age"": 30 },
{ ""Name"": ""Jane"", ""Age"": 25 }
]
}";
// Create JsonLayoutOptions
JsonLayoutOptions options = new JsonLayoutOptions();
// Display current IgnoreArrayTitle value
Console.WriteLine("Current IgnoreArrayTitle value: " + options.IgnoreArrayTitle);
// First import with IgnoreArrayTitle = false (default)
options.IgnoreArrayTitle = false;
JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
Console.WriteLine("Data imported with IgnoreArrayTitle=false. Check cell A1 for 'Employees' title.");
// Clear worksheet for second import
worksheet.Cells.Clear();
// Second import with IgnoreArrayTitle = true
options.IgnoreArrayTitle = true;
JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
Console.WriteLine("Data imported with IgnoreArrayTitle=true. Check cell A1 for direct array values.");
// Save the workbook
workbook.Save("JsonLayoutOptionsIgnoreArrayTitleDemo.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
