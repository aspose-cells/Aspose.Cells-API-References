##Enum DataBarAxisPosition
Aspose.Cells.DataBarAxisPosition enum. Specifies the axis position for a range of cells with conditional formatting as data bars
## DataBarAxisPosition enumeration
Specifies the axis position for a range of cells with conditional formatting as data bars.
```csharp
public enum DataBarAxisPosition
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Display the axis at a variable position based on the ratio of the minimum negative value to the maximum positive value in the range. Positive values are displayed in a left-to-right direction. Negative values are displayed in a right-to-left direction. When all values are positive or all values are negative, no axis is displayed. |
| Midpoint | `1` | Display the axis at the midpoint of the cell regardless of the set of values in the range. Positive values are displayed in a left-to-right direction. Negative values are displayed in a right-to-left direction. |
| None | `2` | No axis is displayed, and both positive and negative values are displayed in the left-to-right direction. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class DataBarAxisPositionDemo
{
public static void DataBarAxisPositionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Accessing the first worksheet in the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Adding a conditional formatting rule
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Setting the conditional format range
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 2,
StartColumn = 0,
EndColumn = 0
};
fcs.AddArea(ca);
// Adding a data bar condition
int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
FormatCondition fc = fcs[conditionIndex];
DataBar dataBar = fc.DataBar;
// Setting properties for the data bar
dataBar.Color = Color.Orange;
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
dataBar.MinCfvo.Value = 30;
dataBar.ShowValue = false;
dataBar.BarBorder.Type = DataBarBorderType.Solid;
dataBar.BarBorder.Color = Color.Plum;
dataBar.BarFillType = DataBarFillType.Solid;
dataBar.AxisColor = Color.Red;
dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
dataBar.NegativeBarFormat.Color = Color.White;
dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
// Putting cell values
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(120);
worksheet.Cells["A3"].PutValue(260);
// Saving the Excel file
workbook.Save("DataBarAxisPositionExample.xlsx");
workbook.Save("DataBarAxisPositionExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
