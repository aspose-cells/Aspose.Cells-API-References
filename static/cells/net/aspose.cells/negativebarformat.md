##Class NegativeBarFormat
Aspose.Cells.NegativeBarFormat class. Represents the color settings of the data bars for negative values that are defined by a data bar conditional formatting rule
## NegativeBarFormat class
Represents the color settings of the data bars for negative values that are defined by a data bar conditional formatting rule.
```csharp
public class NegativeBarFormat
```
## Properties
| Name | Description |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | Gets or sets a FormatColor object that you can use to specify the border color for negative data bars. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | Gets whether to use the same border color as positive data bars. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | Gets or sets whether to use the same fill color as positive data bars. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class NegativeBarFormatDemo
{
public static void NegativeBarFormatExample()
{
// Instantiate a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adds an empty conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Sets the conditional format range
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 10,
StartColumn = 0,
EndColumn = 10
};
fcs.AddArea(ca);
// Adds condition for DataBar
int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
FormatCondition fc = fcs[conditionIndex];
// Get DataBar and set its properties
DataBar dataBar = fc.DataBar;
dataBar.Color = Color.Orange;
dataBar.BarFillType = DataBarFillType.Solid;
dataBar.AxisColor = Color.Red;
dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
// Configure the NegativeBarFormat properties
NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
negativeBarFormat.Color = Color.White;
negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
negativeBarFormat.BorderColor = Color.Yellow;
negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
// Put some values in the cells
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(120);
worksheet.Cells["A3"].PutValue(260);
// Save the workbook
workbook.Save("NegativeBarFormatExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
