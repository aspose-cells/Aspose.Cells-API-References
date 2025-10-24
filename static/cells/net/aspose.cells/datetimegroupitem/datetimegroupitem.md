##DateTimeGroupItem.DateTimeGroupItem
DateTimeGroupItem constructor.
## DateTimeGroupItem constructor
```csharp
public DateTimeGroupItem(DateTimeGroupingType type, int year, int month, int day, int hour,
int minute, int second)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | DateTimeGroupingType |  |
| year | Int32 |  |
| month | Int32 |  |
| day | Int32 |  |
| hour | Int32 |  |
| minute | Int32 |  |
| second | Int32 |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DateTimeGroupItemMethodCtorWithDateTimeGroupingTypeInt32Int32Demo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample datetime data to column A
worksheet.Cells["A1"].PutValue("Order Date");
worksheet.Cells["A2"].PutValue(new DateTime(2023, 3, 15, 9, 30, 15));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 4, 20, 14, 15, 45));
worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 25, 10, 0, 0));
worksheet.Cells["A5"].PutValue(new DateTime(2024, 3, 1, 8, 45, 30));
// Apply autofilter to date column
worksheet.AutoFilter.Range = "A1:A5";
try
{
// Create DateTimeGroupItem for March 2023 grouping
DateTimeGroupItem groupItem = new DateTimeGroupItem(
DateTimeGroupingType.Month, // Group by Month
2023,   // Year
3,      // Month (March)
1,      // Day (ignored in Month grouping)
0,      // Hour
0,      // Minute
0       // Second
);
// Configure filter to show March 2023 dates
FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
filterColumn.FilterType = FilterType.MultipleFilters;
filterColumn.Filter = groupItem;
// Refresh filter to apply changes
worksheet.AutoFilter.Refresh();
Console.WriteLine("DateTimeGroupItem created and filter applied successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Error applying date filter: {ex.Message}");
}
// Save the filtered workbook
workbook.Save("DateTimeGroupItemConstructorDemo.xlsx");
}
}
}
```
### See Also
* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
