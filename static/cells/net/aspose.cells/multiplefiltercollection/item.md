##MultipleFilterCollection.Item
MultipleFilterCollection property. DateTimeGroupItem or a simple object
## MultipleFilterCollection indexer
DateTimeGroupItem or a simple object.
```csharp
public object this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index |  |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MultipleFilterCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Date");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 6));
sheet.Cells["B2"].PutValue(100);
sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 7));
sheet.Cells["B3"].PutValue(200);
sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 8));
sheet.Cells["B4"].PutValue(300);
// Apply auto filter
sheet.AutoFilter.Range = "A1:B4";
sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
sheet.AutoFilter.Refresh();
// Access the filter collection
FilterColumn fc = sheet.AutoFilter.FilterColumns[0];
MultipleFilterCollection m = fc.Filter as MultipleFilterCollection;
// Demonstrate Item property usage
if (m.Count > 0)
{
DateTimeGroupItem dateTimeGroupItem = m[0] as DateTimeGroupItem;
Console.WriteLine($"Filtered day: {dateTimeGroupItem.Day}");
}
// Remove filter
sheet.AutoFilter.RemoveFilter(0);
sheet.AutoFilter.Refresh();
}
}
}
```
### See Also
* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
