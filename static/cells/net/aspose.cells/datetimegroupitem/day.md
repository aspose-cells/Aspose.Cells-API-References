##DateTimeGroupItem.Day
DateTimeGroupItem property. Gets and sets the day of the grouped date time
## DateTimeGroupItem.Day property
Gets and sets the day of the grouped date time.
```csharp
public int Day { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DateTimeGroupItemPropertyDayDemo
{
public static void Run()
{
// Create a DateTimeGroupItem grouped by Year
DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
DateTimeGroupingType.Year,
2023,  // Year
10,    // Month
5,     // Day
14,    // Hour
30,    // Minute
45     // Second
);
// Display initial day value
Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);
// Change the day property
dateTimeGroupItem.Day = 25;
Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);
// Create another DateTimeGroupItem grouped by Day to demonstrate Day property significance
DateTimeGroupItem dayGroupItem = new DateTimeGroupItem(
DateTimeGroupingType.Day,
2023,
10,
15,  // Initial day
0,
0,
0
);
Console.WriteLine("\nDay-grouped item initial Day: " + dayGroupItem.Day);
dayGroupItem.Day = 20;
Console.WriteLine("Day-grouped item modified Day: " + dayGroupItem.Day);
}
}
}
```
### See Also
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
