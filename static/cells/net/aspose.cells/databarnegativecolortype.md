##Enum DataBarNegativeColorType
Aspose.Cells.DataBarNegativeColorType enum. Specifies whether to use the same border and fill color as positive data bars
## DataBarNegativeColorType enumeration
Specifies whether to use the same border and fill color as positive data bars.
```csharp
public enum DataBarNegativeColorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Color | `0` | Use the color specified in the Negative Value and Axis Setting dialog box or by using the ColorType and BorderColorType properties of the NegativeBarFormat object. |
| SameAsPositive | `1` | Use the same color as positive data bars. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DataBarNegativeColorTypeDemo
{
public static void DataBarNegativeColorTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(-20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(-40);
worksheet.Cells["A5"].PutValue(50);
// Add conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
fcs.AddArea(ca);
int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
FormatCondition fc = fcs[conditionIndex];
// Set the data bar properties
DataBar dataBar = fc.DataBar;
dataBar.MinCfvo.Type = FormatConditionValueType.Number;
dataBar.MinCfvo.Value = -50;
dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
dataBar.MaxCfvo.Value = 50;
dataBar.Color = System.Drawing.Color.Green;
// Set negative bar format properties
NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
negativeBarFormat.Color = System.Drawing.Color.Red;
negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;
// Save the workbook
workbook.Save("DataBarNegativeColorTypeExample.xlsx");
workbook.Save("DataBarNegativeColorTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
