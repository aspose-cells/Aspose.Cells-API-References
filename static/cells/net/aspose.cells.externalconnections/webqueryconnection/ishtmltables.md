##WebQueryConnection.IsHtmlTables
WebQueryConnection property. Flag indicating whether web queries should only work on HTML tables
## WebQueryConnection.IsHtmlTables property
Flag indicating whether web queries should only work on HTML tables.
```csharp
public bool IsHtmlTables { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class WebQueryConnectionPropertyIsHtmlTablesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
try
{
// Create web query connection through collection indexer
WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];
Console.WriteLine("Initial IsHtmlTables: " + connection.IsHtmlTables);
connection.IsHtmlTables = true;
Console.WriteLine("Updated IsHtmlTables: " + connection.IsHtmlTables);
workbook.Save("IsHtmlTablesDemo.xlsx");
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
