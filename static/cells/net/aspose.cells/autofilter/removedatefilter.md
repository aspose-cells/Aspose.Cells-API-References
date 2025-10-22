##AutoFilter.RemoveDateFilter
AutoFilter method. Removes a date filter
## AutoFilter.RemoveDateFilter method
Removes a date filter.
```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year,
int month, int day, int hour, int minute, int second)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | DateTimeGroupingType | The grouping type |
| year | Int32 | The year. |
| month | Int32 | The month. |
| day | Int32 | The day. |
| hour | Int32 | The hour. |
| minute | Int32 | The minute. |
| second | Int32 | The second. |
### Remarks
If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodRemoveDateFilterWithInt32DateTimeGroupingTypeInt32Demo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data with dates
sheet.Cells["A1"].PutValue("Date");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 7));
sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 8));
sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 9));
// Apply auto filter
sheet.AutoFilter.Range = "A1:A4";
// Add date filter for day 7
sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
sheet.AutoFilter.Refresh();
// Verify filter is applied
Console.WriteLine("Row 2 hidden: " + sheet.Cells.IsRowHidden(1)); // Should be true
// Remove the date filter
sheet.AutoFilter.RemoveDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
sheet.AutoFilter.Refresh();
// Verify filter is removed
Console.WriteLine("Row 2 hidden after removal: " + sheet.Cells.IsRowHidden(1)); // Should be false
}
}
}
```
### See Also
* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
