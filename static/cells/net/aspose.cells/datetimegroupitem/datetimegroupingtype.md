##DateTimeGroupItem.DateTimeGroupingType
DateTimeGroupItem property. Gets and sets the group type
## DateTimeGroupItem.DateTimeGroupingType property
Gets and sets the group type.
```csharp
public DateTimeGroupingType DateTimeGroupingType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DateTimeGroupItemPropertyDateTimeGroupingTypeDemo
{
public static void Run()
{
// Create an instance of DateTimeGroupItem
DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
DateTimeGroupingType.Year, // Group by Year
2023,                      // Year
10,                       // Month
5,                         // Day
14,                       // Hour
30,                       // Minute
45                        // Second
);
// Display initial properties
Console.WriteLine("Initial Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
Console.WriteLine($"Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}-{dateTimeGroupItem.Day}");
// Change grouping type and date components
dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
dateTimeGroupItem.Year = 2022;
dateTimeGroupItem.Month = 12;
// Display modified properties
Console.WriteLine("Modified Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
Console.WriteLine($"Modified Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}");
}
}
}
```
### See Also
* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
