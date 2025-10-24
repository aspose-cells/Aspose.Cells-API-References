##WebQueryConnection.IsTextDates
WebQueryConnection property. Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates
## WebQueryConnection.IsTextDates property
Flag indicating whether dates should be imported into cells in the worksheet as text rather than dates.
```csharp
public bool IsTextDates { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyIsTextDatesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a web query connection by loading from an existing file
// or accessing an existing connection
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection connection)
{
// Display initial IsTextDates value
Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
// Set IsTextDates to true
connection.IsTextDates = true;
Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
// Set IsTextDates back to false
connection.IsTextDates = false;
Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
// Save the workbook with the web query connection
workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
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
