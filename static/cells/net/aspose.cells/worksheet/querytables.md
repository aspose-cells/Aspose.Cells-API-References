##Worksheet.QueryTables
Worksheet property. Gets QueryTableCollection in the worksheet
## Worksheet.QueryTables property
Gets [`QueryTableCollection`](../../querytablecollection/) in the worksheet.
```csharp
public QueryTableCollection QueryTables { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyQueryTablesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(1.8);
// Get the first query table (since we can't add new ones directly)
// Note: QueryTables collection is read-only in this API version
if (worksheet.QueryTables.Count > 0)
{
QueryTable queryTable = worksheet.QueryTables[0];
// Display query table information
Console.WriteLine("Query Table Name: " + queryTable.Name);
Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
Console.WriteLine("Number of Query Tables: " + worksheet.QueryTables.Count);
}
else
{
Console.WriteLine("No query tables found in the worksheet.");
}
// Save the workbook
workbook.Save("QueryTableDemo.xlsx");
}
}
}
```
### See Also
* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
