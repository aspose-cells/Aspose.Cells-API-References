##DateTimeGroupItem.Year
DateTimeGroupItem property. Gets and sets the year of the grouped date time
## DateTimeGroupItem.Year property
Gets and sets the year of the grouped date time.
```csharp
public int Year { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DateTimeGroupItemPropertyYearDemo
{
public static void Run()
{
// Create a DateTimeGroupItem grouped by Year
DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
DateTimeGroupingType.Year,
2023,  // Year
1,     // Month (ignored when grouping by Year)
1,     // Day (ignored)
0,     // Hour (ignored)
0,     // Minute (ignored)
0      // Second (ignored)
);
// Display initial Year value
Console.WriteLine("Initial Year: " + dateTimeGroup.Year);
// Modify the Year property
dateTimeGroup.Year = 2024;
// Display modified Year value
Console.WriteLine("Modified Year: " + dateTimeGroup.Year);
// Demonstrate that other properties are ignored when grouping by Year
dateTimeGroup.Month = 12;
Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
}
}
}
```
### See Also
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
