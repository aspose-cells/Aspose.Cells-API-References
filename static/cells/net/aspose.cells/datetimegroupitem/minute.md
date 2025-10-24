##DateTimeGroupItem.Minute
DateTimeGroupItem property. Gets and sets the minute of the grouped date time
## DateTimeGroupItem.Minute property
Gets and sets the minute of the grouped date time.
```csharp
public int Minute { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DateTimeGroupItemPropertyMinuteDemo
{
public static void Run()
{
// Create a DateTimeGroupItem with initial values
DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
DateTimeGroupingType.Year,
2023,
10,
5,
14,
30,
45
);
// Display initial minute value
Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);
// Change the minute value
dateTimeGroupItem.Minute = 15;
// Display modified minute value
Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);
// Create a new DateTimeGroupItem with only minute grouping
DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
DateTimeGroupingType.Minute,
0, 0, 0, 0, 45, 0
);
// Display minute from minute grouping
Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
}
}
}
```
### See Also
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
