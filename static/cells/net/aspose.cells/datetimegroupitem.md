##Class DateTimeGroupItem
Aspose.Cells.DateTimeGroupItem class. Represents the datetimes group setting
## DateTimeGroupItem class
Represents the datetime's group setting.
```csharp
public class DateTimeGroupItem
```
## Constructors
| Name | Description |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |
## Properties
| Name | Description |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | Gets and sets the group type. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | Gets and sets the day of the grouped date time. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | Gets and sets the hour of the grouped date time. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | Gets and sets the minute of the grouped date time. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | Gets the min value. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | Gets and sets the month of the grouped date time. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | Gets and sets the second of the grouped date time. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | Gets and sets the year of the grouped date time. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DateTimeGroupItemDemo
{
public static void DateTimeGroupItemExample()
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
// Accessing properties
Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
Console.WriteLine("Year: " + dateTimeGroupItem.Year);
Console.WriteLine("Month: " + dateTimeGroupItem.Month);
Console.WriteLine("Day: " + dateTimeGroupItem.Day);
Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
Console.WriteLine("Second: " + dateTimeGroupItem.Second);
// Modifying properties
dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
dateTimeGroupItem.Year = 2022;
dateTimeGroupItem.Month = 12;
dateTimeGroupItem.Day = 25;
dateTimeGroupItem.Hour = 10;
dateTimeGroupItem.Minute = 15;
dateTimeGroupItem.Second = 30;
// Accessing modified properties
Console.WriteLine("Modified DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
Console.WriteLine("Modified Year: " + dateTimeGroupItem.Year);
Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);
Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);
Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);
Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
