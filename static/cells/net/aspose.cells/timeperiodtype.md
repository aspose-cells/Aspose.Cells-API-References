##Enum TimePeriodType
Aspose.Cells.TimePeriodType enum. Used in a FormatConditionType.TimePeriod conditional formatting rule. These are dynamic time periods which change based on the date the conditional formatting is refreshed / applied
## TimePeriodType enumeration
Used in a FormatConditionType.TimePeriod conditional formatting rule. These are dynamic time periods, which change based on the date the conditional formatting is refreshed / applied.
```csharp
public enum TimePeriodType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Today | `0` | Today's date. |
| Yesterday | `1` | Yesterday's date. |
| Tomorrow | `2` | Tomorrow's date. |
| Last7Days | `3` | A date in the last seven days. |
| ThisMonth | `4` | A date occurring in this calendar month. |
| LastMonth | `5` | A date occurring in the last calendar month. |
| NextMonth | `6` | A date occurring in the next calendar month. |
| ThisWeek | `7` | A date occurring this week. |
| LastWeek | `8` | A date occurring last week. |
| NextWeek | `9` | A date occurring next week. |
| ThisYear | `10` | A date occurring this year. Only for .ods. |
| LastYear | `11` | A date occurring last year. Only for .ods. |
| NextYear | `12` | A date occurring next year. Only for .ods. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class TimePeriodTypeDemo
{
public static void TimePeriodTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a conditional formatting rule
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Define the cell area for the conditional formatting
CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
fcs.AddArea(ca);
// Add a condition for the time period
int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;
// Set the time period type
fc.TimePeriod = TimePeriodType.Today;
// Save the workbook
workbook.Save("TimePeriodTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
