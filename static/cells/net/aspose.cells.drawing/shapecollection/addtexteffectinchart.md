##ShapeCollection.AddTextEffectInChart
ShapeCollection method. Inserts a WordArt object to the chart
## ShapeCollection.AddTextEffectInChart method
Inserts a WordArt object to the chart
```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName,
int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| effect | MsoPresetTextEffect | The mso preset text effect type. |
| text | String | The WordArt text. |
| fontName | String | The font name. |
| size | Int32 | The font size |
| fontBold | Boolean | Indicates whether font is bold. |
| fontItalic | Boolean | Indicates whether font is italic. |
| top | Int32 | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | Int32 | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| height | Int32 | Represents the height of shape, in units of 1/4000 of the chart area. |
| width | Int32 | Represents the width of shape, in units of 1/4000 of the chart area. |
### Return Value
Returns a Shape object that represents the new WordArt object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddTextEffectInChartWithMsoPresetTextEffectStringStrinDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet and add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
// Add WordArt to the chart
Shape wordart = chart.Shapes.AddTextEffectInChart(
MsoPresetTextEffect.TextEffect2,
"SAMPLE TEXT",
"Arial Black",
36,
false,
false,
100,  // Left position
100,  // Top position
300,  // Width
200); // Height
// Customize the WordArt appearance
wordart.FillFormat.Transparency = 0.7;
wordart.LineFormat.IsVisible = false;
// Save the workbook
workbook.Save("WordArtInChart.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
