##WebQueryConnection.IsXl97
WebQueryConnection property. This flag exists for backward compatibility with older existing spreadsheet files and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored
## WebQueryConnection.IsXl97 property
This flag exists for backward compatibility with older existing spreadsheet files, and is set to true if this web query was created in Microsoft Excel 97. This is an optional attribute that can be ignored.
```csharp
public bool IsXl97 { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyIsXl97Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a worksheet with some data to make the example meaningful
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Sample Data";
// Create a web query connection by loading from an existing file or creating properly
// Since we can't create WebQueryConnection directly, we'll access an existing one
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection connection)
{
// Display initial IsXl97 value
Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
// Set IsXl97 to true (since it's read-write)
connection.IsXl97 = true;
Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
// Set IsXl97 back to false
connection.IsXl97 = false;
Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
// Save the workbook
workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
}
else
{
Console.WriteLine("No web query connections found in the workbook.");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
