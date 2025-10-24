##Class DataBar
Aspose.Cells.DataBar class. Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells
## DataBar class
Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.
```csharp
public class DataBar
```
## Properties
| Name | Description |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | Gets the color of the axis for cells with conditional formatting as data bars. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | Gets an object that specifies the border of a data bar. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | Gets or sets how a data bar is filled with color. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | Get or set this DataBar's Color. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | Gets or sets the direction the databar is displayed. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | Represents the max length of data bar . |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | Represents the min length of data bar . |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |
## Methods
| Name | Description |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | Render data bar in cell to image byte array. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class DataBarDemo
{
public static void DataBarExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Adds an empty conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
// Sets the conditional format range
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 2,
StartColumn = 0,
EndColumn = 0
};
fcs.AddArea(ca);
// Adds condition
int idx = fcs.AddCondition(FormatConditionType.DataBar);
FormatCondition cond = fcs[idx];
// Get DataBar
DataBar dataBar = cond.DataBar;
// Set DataBar properties
dataBar.Color = Color.Orange;
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
dataBar.MinCfvo.Value = 30;
dataBar.ShowValue = false;
dataBar.BarBorder.Type = DataBarBorderType.Solid;
dataBar.BarBorder.Color = Color.Plum;
dataBar.BarFillType = DataBarFillType.Solid;
dataBar.AxisColor = Color.Red;
dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
dataBar.NegativeBarFormat.Color = Color.White;
dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
// Put Cell Values
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
cell1.PutValue(10);
Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
cell2.PutValue(120);
Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
cell3.PutValue(260);
// Saving the Excel file
workbook.Save("DataBarExample.xlsx");
workbook.Save("DataBarExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
