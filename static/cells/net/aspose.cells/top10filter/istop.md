##Top10Filter.IsTop
Top10Filter property. Indicates whether its top filter
## Top10Filter.IsTop property
Indicates whether it's top filter.
```csharp
public bool IsTop { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class Top10FilterPropertyIsTopDemo
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
}
// Apply top 5 filter
worksheet.AutoFilter.Range = "B6:B16";
worksheet.AutoFilter.FilterTop10(0, true, false, 5);
// Get the filter and check IsTop property
Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
Console.WriteLine("IsTop: " + filter.IsTop); // Should output "True"
Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output "False"
// Refresh filter and check hidden rows
worksheet.AutoFilter.Refresh();
for (int i = 6; i <= 16; i++)
{
Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
}
}
}
}
```
### See Also
* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
