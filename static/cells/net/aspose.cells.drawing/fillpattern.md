##Enum FillPattern
Aspose.Cells.Drawing.FillPattern enum. Enumerates shape fill pattern types
## FillPattern enumeration
Enumerates shape fill pattern types.
```csharp
public enum FillPattern
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Represents no background. |
| Solid | `1` | Represents solid pattern. |
| Gray5 | `2` | Represents 5% gray pattern. |
| Gray10 | `3` | Represents 10% gray pattern. |
| Gray20 | `4` | Represents 20% gray pattern. |
| Gray30 | `5` | Represents 30% gray pattern. |
| Gray40 | `6` | Represents 40% gray pattern. |
| Gray50 | `7` | Represents 50% gray pattern. |
| Gray60 | `8` | Represents 60% gray pattern. |
| Gray70 | `9` | Represents 70% gray pattern. |
| Gray75 | `10` | Represents 75% gray pattern. |
| Gray80 | `11` | Represents 80% gray pattern. |
| Gray90 | `12` | Represents 90% gray pattern. |
| Gray25 | `13` | Represents 25% gray pattern. |
| LightDownwardDiagonal | `14` | Represents light downward diagonal pattern. |
| LightUpwardDiagonal | `15` | Represents light upward diagonal pattern. |
| DarkDownwardDiagonal | `16` | Represents dark downward diagonal pattern. |
| DarkUpwardDiagonal | `17` | Represents dark upward diagonal pattern. |
| WideDownwardDiagonal | `18` | Represents wide downward diagonal pattern. |
| WideUpwardDiagonal | `19` | Represents wide upward diagonal pattern. |
| LightVertical | `20` | Represents light vertical pattern. |
| LightHorizontal | `21` | Represents light horizontal pattern. |
| NarrowVertical | `22` | Represents narrow vertical pattern. |
| NarrowHorizontal | `23` | Represents narrow horizontal pattern. |
| DarkVertical | `24` | Represents dark vertical pattern. |
| DarkHorizontal | `25` | Represents dark horizontal pattern. |
| DashedDownwardDiagonal | `26` | Represents dashed downward diagonal pattern. |
| DashedUpwardDiagonal | `27` | Represents dashed upward diagonal pattern. |
| DashedVertical | `28` | Represents dashed vertical pattern. |
| DashedHorizontal | `29` | Represents dashed horizontal pattern. |
| SmallConfetti | `30` | Represents small confetti pattern. |
| LargeConfetti | `31` | Represents large confetti pattern. |
| ZigZag | `32` | Represents zig zag pattern. |
| Wave | `33` | Represents wave pattern. |
| DiagonalBrick | `34` | Represents diagonal brick pattern. |
| HorizontalBrick | `35` | Represents horizontal brick pattern. |
| Weave | `36` | Represents weave pattern. |
| Plaid | `37` | Represents plaid pattern. |
| Divot | `38` | Represents divot pattern. |
| DottedGrid | `39` | Represents dotted grid pattern. |
| DottedDiamond | `40` | Represents dotted diamond pattern. |
| Shingle | `41` | Represents shingle pattern. |
| Trellis | `42` | Represents trellis pattern. |
| Sphere | `43` | Represents sphere pattern. |
| SmallGrid | `44` | Represents small grid pattern. |
| LargeGrid | `45` | Represents large grid pattern. |
| SmallCheckerBoard | `46` | Represents small checker board pattern. |
| LargeCheckerBoard | `47` | Represents large checker board pattern. |
| OutlinedDiamond | `48` | Represents outlined diamond pattern. |
| SolidDiamond | `49` | Represents solid diamond pattern. |
| Unknown | `50` | Represents unknown pattern. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassFillPatternDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set fill pattern for the first series
Series series = chart.NSeries[0];
series.Area.FillFormat.Pattern = FillPattern.Plaid;
// Save the workbook
workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
