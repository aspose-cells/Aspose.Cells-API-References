##Top10Filter.Items
Top10Filter property. Gets and sets the items of the filter
## Top10Filter.Items property
Gets and sets the items of the filter.
```csharp
public int Items { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class Top10FilterPropertyItemsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruits");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["A5"].PutValue("Grapes");
worksheet.Cells["A6"].PutValue("Mango");
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:A6", "C1", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Apply top 10 filter
pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
// Get the filter and demonstrate Items property
PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
int itemsCount = filter.GetTop10Value().Items;
Console.WriteLine("Top 10 Filter Items Count: " + itemsCount);
}
}
}
```
### See Also
* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
