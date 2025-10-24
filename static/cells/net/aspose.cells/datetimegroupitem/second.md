##DateTimeGroupItem.Second
DateTimeGroupItem property. Gets and sets the second of the grouped date time
## DateTimeGroupItem.Second property
Gets and sets the second of the grouped date time.
```csharp
public int Second { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DateTimeGroupItemPropertySecondDemo
{
public static void Run()
{
// Create an instance of DateTimeGroupItem
DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
DateTimeGroupingType.Year, // Group by Year
2023,                      // Year
10,                        // Month
5,                         // Day
14,                        // Hour
30,                        // Minute
45                         // Second
);
// Display initial second value
Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);
// Modify the second value
dateTimeGroupItem.Second = 50;
Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);
// Create another instance with different second value
DateTimeGroupItem anotherItem = new DateTimeGroupItem(
DateTimeGroupingType.Day,
2023,
10,
5,
14,
30,
0  // Second set to 0
);
Console.WriteLine("Another Item Second: " + anotherItem.Second);
}
}
}
```
### See Also
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
