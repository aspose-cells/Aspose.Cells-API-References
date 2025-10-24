##JsonLayoutOptions.IgnoreObjectTitle
JsonLayoutOptions property. Indicates whether ignore title if object is a property of object
## JsonLayoutOptions.IgnoreObjectTitle property
Indicates whether ignore title if object is a property of object.
```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
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
public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample JSON data with object titles
string json = @"{
""Employees"": {
""Employee"": [
{ ""Name"": ""John"", ""Age"": 30 },
{ ""Name"": ""Jane"", ""Age"": 25 }
]
}
}";
// Create JsonLayoutOptions
JsonLayoutOptions options = new JsonLayoutOptions();
// Display current IgnoreObjectTitle value
Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);
// Set to ignore object titles
options.IgnoreObjectTitle = true;
Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);
// Import JSON with IgnoreObjectTitle = true
JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
// Save with ignored titles
workbook.Save("IgnoreObjectTitle_True.xlsx");
// Reset the worksheet
worksheet.Cells.Clear();
// Set to include object titles
options.IgnoreObjectTitle = false;
Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);
// Import JSON with IgnoreObjectTitle = false
JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
// Save with included titles
workbook.Save("IgnoreObjectTitle_False.xlsx");
}
}
}
```
### See Also
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
