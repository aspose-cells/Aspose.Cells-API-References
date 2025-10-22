##Class Top10Filter
Aspose.Cells.Top10Filter class. Represents the top 10 filter
## Top10Filter class
Represents the top 10 filter.
```csharp
public class Top10Filter
```
## Properties
| Name | Description |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } |  |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Indicates whether the items is percent. |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Indicates whether it's top filter. |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Gets and sets the items of the filter. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassTop10FilterDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["B6"].PutValue("Value");
for (int i = 7; i <= 16; i++)
{
worksheet.Cells["B" + i].PutValue(20 - i);
worksheet.Cells["C" + i].PutValue("Item " + (i-6));
}
// Apply auto filter and top 10 filter
worksheet.AutoFilter.Range = "B6:C16";
worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
// Get the Top10Filter and verify its properties
Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
Console.WriteLine("IsTop: " + filter.IsTop);
Console.WriteLine("IsPercent: " + filter.IsPercent);
Console.WriteLine("Items: " + filter.Items);
// Refresh the filter and check hidden rows
worksheet.AutoFilter.Refresh();
for (int i = 6; i <= 16; i++)
{
Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
}
// Save the workbook
workbook.Save("Top10FilterDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
