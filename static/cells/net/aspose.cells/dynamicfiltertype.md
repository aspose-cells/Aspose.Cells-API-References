##Enum DynamicFilterType
Aspose.Cells.DynamicFilterType enum. Dynamic filter type
## DynamicFilterType enumeration
Dynamic filter type.
```csharp
public enum DynamicFilterType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| AboveAverage | `0` | Shows values that are above average. |
| BelowAverage | `1` | Shows values that are below average. |
| LastMonth | `2` | Shows last month's dates. |
| LastQuarter | `3` | Shows last quarter's dates. |
| LastWeek | `4` | Shows last week's dates. |
| LastYear | `5` | Shows last year's dates. |
| January | `6` | Shows the dates that are in January, regardless of year. |
| October | `7` | Shows the dates that are in October, regardless of year. |
| November | `8` | Shows the dates that are in November, regardless of year. |
| December | `9` | Shows the dates that are in December, regardless of year. |
| February | `10` | Shows the dates that are in February, regardless of year. |
| March | `11` | Shows the dates that are in March, regardless of year. |
| April | `12` | Shows the dates that are in April, regardless of year. |
| May | `13` | Shows the dates that are in May, regardless of year. |
| June | `14` | Shows the dates that are in June, regardless of year. |
| July | `15` | Shows the dates that are in July, regardless of year. |
| August | `16` | Shows the dates that are in August, regardless of year. |
| September | `17` | Shows the dates that are in September, regardless of year. |
| NextMonth | `18` | Shows next month's dates. |
| NextQuarter | `19` | Shows next quarter's dates. |
| NextWeek | `20` | Shows next week's dates. |
| NextYear | `21` | Shows next year's dates. |
| None | `22` | None. |
| Quarter1 | `23` | Shows the dates that are in the 1st quarter, regardless of year. |
| Quarter2 | `24` | Shows the dates that are in the 2nd quarter, regardless of year. |
| Quarter3 | `25` | Shows the dates that are in the 3rd quarter, regardless of year. |
| Quarter4 | `26` | Shows the dates that are in the 4th quarter, regardless of year. |
| ThisMonth | `27` | Shows this month's dates. |
| ThisQuarter | `28` | Shows this quarter's dates. |
| ThisWeek | `29` | Shows this week's dates. |
| ThisYear | `30` | Shows this year's dates. |
| Today | `31` | Shows today's dates. |
| Tomorrow | `32` | Shows tomorrow's dates. |
| YearToDate | `33` | Shows the dates between the beginning of the year and today, inclusive. |
| Yesterday | `34` | Shows yesterday's dates. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DynamicFilterTypeDemo
{
public static void DynamicFilterTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
worksheet.Cells["B6"].PutValue(50);
// Apply auto filter to the worksheet
worksheet.AutoFilter.SetRange(0, 0, 5);
// Apply a dynamic filter to show only dates in March
worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
// Save the workbook
workbook.Save("DynamicFilterTypeExample.xlsx");
workbook.Save("DynamicFilterTypeExample.pdf");
// Output the results
Console.WriteLine("Dynamic filter applied to show only dates in March.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
