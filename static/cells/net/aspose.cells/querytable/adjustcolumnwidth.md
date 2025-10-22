##QueryTable.AdjustColumnWidth
QueryTable property. Returns or sets the AdjustColumnWidth of the object
## QueryTable.AdjustColumnWidth property
Returns or sets the AdjustColumnWidth of the object.
```csharp
public bool AdjustColumnWidth { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class QueryTablePropertyAdjustColumnWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with varying column widths
worksheet.Cells["A1"].PutValue("Narrow Column");
worksheet.Cells["B1"].PutValue("Wide Column Data");
worksheet.Cells["A2"].PutValue("Short");
worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");
// Manually set column widths
worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data
// Create a query table (simulated since actual creation requires external data source)
QueryTable queryTable = worksheet.QueryTables[0];
// Display current AdjustColumnWidth value
Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);
// Set AdjustColumnWidth to true and demonstrate effect
queryTable.AdjustColumnWidth = true;
Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");
// Simulate refreshing the query table (would normally adjust column widths)
// In a real scenario, this would happen when the query table refreshes its data
Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));
// Set AdjustColumnWidth to false and demonstrate effect
queryTable.AdjustColumnWidth = false;
Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
// Simulate refreshing again (would now preserve original column widths)
Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));
// Save the workbook
workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
}
}
}
```
### See Also
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
