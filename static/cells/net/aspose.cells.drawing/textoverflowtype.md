##Enum TextOverflowType
Aspose.Cells.Drawing.TextOverflowType enum. Represents the way the text vertical or horizontal overflow
## TextOverflowType enumeration
Represents the way the text vertical or horizontal overflow.
```csharp
public enum TextOverflowType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Clip | `0` | Pay attention to top and bottom barriers. Provide no indication that there is text which is not visible. |
| Ellipsis | `1` | Pay attention to top and bottom barriers. Use an ellipsis to denote that there is text which is not visible. Only for vertical overflow. |
| Overflow | `2` | Overflow the text and pay no attention to top and bottom barriers. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DrawingClassTextOverflowTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add a text box to the chart
TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);
// Set text box properties
textBox.TextBody.TextAlignment.AutoSize = false;
textBox.Text = "This is a long text that will demonstrate text overflow handling";
// Set text overflow type
textBox.TextVerticalOverflow = TextOverflowType.Clip;
// Save the workbook
workbook.Save("TextOverflowTypeDemo_out.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
