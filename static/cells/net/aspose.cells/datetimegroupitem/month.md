##DateTimeGroupItem.Month
DateTimeGroupItem property. Gets and sets the month of the grouped date time
## DateTimeGroupItem.Month property
Gets and sets the month of the grouped date time.
```csharp
public int Month { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DateTimeGroupItemPropertyMonthDemo
{
public static void Run()
{
// Create a DateTimeGroupItem grouped by Month
DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
DateTimeGroupingType.Month,
2023,
10,
1,
0,
0,
0
);
// Display initial month value
Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);
// Change the month value
dateTimeGroupItem.Month = 12;
Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);
// Create another DateTimeGroupItem with different grouping
DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
DateTimeGroupingType.Year,
2023,
1,
1,
0,
0,
0
);
// Show that Month property is still accessible even when grouped by Year
Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
}
}
}
```
### See Also
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
