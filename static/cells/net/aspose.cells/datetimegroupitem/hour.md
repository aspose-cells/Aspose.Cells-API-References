##DateTimeGroupItem.Hour
DateTimeGroupItem property. Gets and sets the hour of the grouped date time
## DateTimeGroupItem.Hour property
Gets and sets the hour of the grouped date time.
```csharp
public int Hour { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DateTimeGroupItemPropertyHourDemo
{
public static void Run()
{
// Create a DateTimeGroupItem with hour grouping
DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
DateTimeGroupingType.Hour,
2023,  // Year
10,     // Month
5,      // Day
14,     // Hour
0,      // Minute
0      // Second
);
// Display initial hour value
Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);
// Modify the hour property
dateTimeGroupItem.Hour = 18;
// Display modified hour value
Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
}
}
}
```
### See Also
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
