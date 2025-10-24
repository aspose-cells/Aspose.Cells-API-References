##Enum WeightType
Aspose.Cells.Drawing.WeightType enum. Enumerates the weight types for a picture border or a chart line
## WeightType enumeration
Enumerates the weight types for a picture border or a chart line.
```csharp
public enum WeightType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| HairLine | `-1` | Represents the weight of hair line. |
| MediumLine | `1` | Represents the weight of medium line. |
| SingleLine | `0` | Represents the weight of single line. |
| WideLine | `2` | Represents the weight of wide line. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassWeightTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a chart and get its chart area
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
Chart chart = worksheet.Charts[chartIndex];
ChartArea chartArea = chart.ChartArea;
// Set border weight type
chartArea.Border.Weight = WeightType.WideLine;
// Verify the weight type
Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
// Save the workbook
workbook.Save("WeightTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
