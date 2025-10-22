##Class ConditionalFormattingResult
Aspose.Cells.ConditionalFormattingResult class. Represents the result of conditional formatting which applies to a cell
## ConditionalFormattingResult class
Represents the result of conditional formatting which applies to a cell.
```csharp
public class ConditionalFormattingResult
```
## Properties
| Name | Description |
| --- | --- |
| [ColorScaleResult](../../aspose.cells/conditionalformattingresult/colorscaleresult/) { get; } | Gets the display color of color scale. |
| [ConditionalFormattingColorScale](../../aspose.cells/conditionalformattingresult/conditionalformattingcolorscale/) { get; } | Gets the ColorScale object. |
| [ConditionalFormattingDataBar](../../aspose.cells/conditionalformattingresult/conditionalformattingdatabar/) { get; } | Gets the DataBar object. |
| [ConditionalFormattingIcon](../../aspose.cells/conditionalformattingresult/conditionalformattingicon/) { get; } | Gets the image of icon set. |
| [ConditionalStyle](../../aspose.cells/conditionalformattingresult/conditionalstyle/) { get; } | Gets the conditional result style. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class ConditionalFormattingResultDemo
{
public static void ConditionalFormattingResultExample()
{
// Instantiate a workbook object
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
// Set ColorScale properties
fc.ColorScale.Is3ColorScale = true;
fc.ColorScale.MinColor = Color.Red;
fc.ColorScale.MidColor = Color.Yellow;
fc.ColorScale.MaxColor = Color.Green;
// Apply some values to the cells
for (int i = 0; i <= 10; i++)
{
for (int j = 0; j <= 10; j++)
{
worksheet.Cells[i, j].PutValue(i * j);
}
}
// Get the conditional formatting result for a specific cell
Cell cell = worksheet.Cells["A1"];
ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();
// Access the properties of ConditionalFormattingResult
Style conditionalStyle = cfr.ConditionalStyle;
ConditionalFormattingIcon icon = cfr.ConditionalFormattingIcon;
DataBar dataBar = cfr.ConditionalFormattingDataBar;
ColorScale colorScale = cfr.ConditionalFormattingColorScale;
Color colorScaleResult = cfr.ColorScaleResult;
// Display some of the properties
Console.WriteLine("Conditional Style Background Color: " + (conditionalStyle != null ? conditionalStyle.BackgroundColor : Color.Empty));
Console.WriteLine("Conditional Formatting Icon Type: " + (icon != null ? icon.Type.ToString() : "No Icon"));
Console.WriteLine("Conditional Formatting DataBar Color: " + (dataBar != null ? dataBar.Color.ToString() : "No DataBar"));
Console.WriteLine("Conditional Formatting ColorScale Min Color: " + (colorScale != null ? colorScale.MinColor.ToString() : "No ColorScale"));
Console.WriteLine("Color Scale Result: " + colorScaleResult);
// Save the workbook
workbook.Save("ConditionalFormattingResultExample.xlsx");
workbook.Save("ConditionalFormattingResultExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
