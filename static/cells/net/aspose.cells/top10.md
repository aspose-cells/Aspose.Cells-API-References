##Class Top10
Aspose.Cells.Top10 class. Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket as specified
## Top10 class
Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.
```csharp
public class Top10
```
## Constructors
| Name | Description |
| --- | --- |
| [Top10](top10/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class Top10Demo
{
public static void Top10Example()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Adds an empty conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
// Sets the conditional format range
CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
fcs.AddArea(ca);
// Adds condition
int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
// Setting properties
Top10 top10 = fc.Top10;
top10.IsPercent = false;
top10.IsBottom = false;
top10.Rank = 5;
// Saving the Excel file
workbook.Save("Top10Example.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
