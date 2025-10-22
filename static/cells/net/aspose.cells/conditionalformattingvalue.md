##Class ConditionalFormattingValue
Aspose.Cells.ConditionalFormattingValue class. Describes the values of the interpolation points in a gradient scale dataBar or iconSet
## ConditionalFormattingValue class
Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.
```csharp
public class ConditionalFormattingValue
```
## Properties
| Name | Description |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | Get or set the value of this conditional formatting value object. It should be used in conjunction with Type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class ConditionalFormattingValueDemo
{
public static void ConditionalFormattingValueExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adds an empty conditional formatting
int index = worksheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
// Sets the conditional format range
CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
fcs.AddArea(ca);
// Adds condition
int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
FormatCondition fc = fcs[conditionIndex];
// Setting properties for ColorScale
fc.ColorScale.Is3ColorScale = true;
// Setting min value
fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
fc.ColorScale.MinCfvo.Value = null;
fc.ColorScale.MinColor = Color.Blue;
// Setting mid value
fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
fc.ColorScale.MidCfvo.Value = 50;
fc.ColorScale.MidColor = Color.Yellow;
// Setting max value
fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
fc.ColorScale.MaxCfvo.Value = null;
fc.ColorScale.MaxColor = Color.Red;
// Save the workbook
workbook.Save("ConditionalFormattingValueExample.xlsx");
workbook.Save("ConditionalFormattingValueExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
