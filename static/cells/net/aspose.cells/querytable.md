##Class QueryTable
Aspose.Cells.QueryTable class. Represents QueryTable information
## QueryTable class
Represents QueryTable information.
```csharp
public class QueryTable
```
## Properties
| Name | Description |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Returns or sets the AdjustColumnWidth of the object. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Gets the connection id of the query table. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | Gets the relate external connection. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Gets the name of querytable. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Returns or sets the PreserveFormatting of the object. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Gets the range of the result. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassQueryTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a query table (simulating external data)
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Mary");
// Check if there are any query tables in the worksheet
if (worksheet.QueryTables.Count > 0)
{
// Get the first query table
QueryTable qt = worksheet.QueryTables[0];
// Display query table properties
Console.WriteLine("Query Table Name: " + qt.Name);
Console.WriteLine("Connection ID: " + qt.ConnectionId);
Console.WriteLine("Result Range: " + qt.ResultRange.Address);
Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
// Modify some properties
qt.PreserveFormatting = true;
qt.AdjustColumnWidth = false;
}
else
{
Console.WriteLine("No query tables found in the worksheet.");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
