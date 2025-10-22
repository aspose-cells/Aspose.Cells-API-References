##WorksheetCollection.RefreshAll
WorksheetCollection method. Refresh all pivot tables and charts with pivot source
## WorksheetCollection.RefreshAll method
Refresh all pivot tables and charts with pivot source.
```csharp
public void RefreshAll()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodRefreshAllDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formulas
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["B3"].PutValue(1.8);
// Add formulas that will be refreshed
worksheet.Cells["C1"].PutValue("Total");
worksheet.Cells["C2"].PutValue("=SUM(B2:B3)");
// Change some values
worksheet.Cells["B2"].PutValue(3.0);
worksheet.Cells["B3"].PutValue(2.0);
// Refresh all formulas in all worksheets
workbook.Worksheets.RefreshAll();
// Output the refreshed total
Console.WriteLine("Refreshed total: " + worksheet.Cells["C2"].StringValue);
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
