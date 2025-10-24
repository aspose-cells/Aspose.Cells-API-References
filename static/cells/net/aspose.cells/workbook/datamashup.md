##Workbook.DataMashup
Workbook property. Gets mashup data
## Workbook.DataMashup property
Gets mashup data.
```csharp
public DataMashup DataMashup { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class WorkbookPropertyDataMashupDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to trigger Power Query
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(150);
// Save to a file
string sourcePath = "source.xlsx";
workbook.Save(sourcePath);
// Reopen the workbook to access DataMashup
workbook = new Workbook(sourcePath);
// Access Power Query formulas through DataMashup property
var queries = workbook.DataMashup.PowerQueryFormulas;
// Output basic information about queries
Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
// If there are any queries, show details of the first one
if (queries.Count > 0)
{
foreach (var query in queries)
{
Console.WriteLine($"Query Name: {query.Name}");
Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
break; // Just show first query for demo
}
}
// Save to a new file
string destPath = "output.xlsx";
workbook.Save(destPath);
}
}
}
```
### See Also
* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
