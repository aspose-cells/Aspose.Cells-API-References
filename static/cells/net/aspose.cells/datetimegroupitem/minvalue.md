##DateTimeGroupItem.MinValue
DateTimeGroupItem property. Gets the min value
## DateTimeGroupItem.MinValue property
Gets the min value.
```csharp
public DateTime MinValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DateTimeGroupItemPropertyMinValueDemo
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
// Demonstrate MinValue property
Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
// Show other properties for context
Console.WriteLine("Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
Console.WriteLine("Date Components: {0}-{1}-{2} {3}:{4}:{5}",
dateTimeGroupItem.Year,
dateTimeGroupItem.Month,
dateTimeGroupItem.Day,
dateTimeGroupItem.Hour,
dateTimeGroupItem.Minute,
dateTimeGroupItem.Second);
}
}
}
```
### See Also
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
