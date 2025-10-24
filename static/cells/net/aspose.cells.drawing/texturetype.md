##Enum TextureType
Aspose.Cells.Drawing.TextureType enum. Represents the preset texture type
## TextureType enumeration
Represents the preset texture type.
```csharp
public enum TextureType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| BlueTissuePaper | `0` | Represents Blue Tissue Paper texture type. |
| Bouquet | `1` | Represents Bouquet texture type. |
| BrownMarble | `2` | Represents Brown Marble texture type. |
| Canvas | `3` | Represents Canvas texture type. |
| Cork | `4` | Represents Cork texture type. |
| Denim | `5` | Represents Denim texture type. |
| FishFossil | `6` | Represents Fish Fossil texture type. |
| Granite | `7` | Represents Granite texture type. |
| GreenMarble | `8` | Represents Green Marble texture type. |
| MediumWood | `9` | Represents Medium Wood texture type. |
| Newsprint | `10` | Represents Newsprint texture type. |
| Oak | `11` | Represents Oak texture type. |
| PaperBag | `12` | Represents Paper Bag texture type. |
| Papyrus | `13` | Represents Papyrus texture type. |
| Parchment | `14` | Represents Parchment texture type. |
| PinkTissuePaper | `15` | Represents Pink Tissue Paper texture type. |
| PurpleMesh | `16` | Represents Purple Mesh texture type. |
| RecycledPaper | `17` | Represents Recycled Paper texture type. |
| Sand | `18` | Represents Sand texture type. |
| Stationery | `19` | Represents Stationery texture type. |
| Walnut | `20` | Represents Walnut Droplets texture type. |
| WaterDroplets | `21` | Represents Water Droplets texture type. |
| WhiteMarble | `22` | Represents White Marble texture type. |
| WovenMat | `23` | Represents Woven Mat texture type. |
| Unknown | `24` | Represents Unknown texture type. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassTextureTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for chart
sheet.Cells["A1"].PutValue("Item");
sheet.Cells["A2"].PutValue("Product A");
sheet.Cells["A3"].PutValue("Product B");
sheet.Cells["A4"].PutValue("Product C");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(1000);
sheet.Cells["B3"].PutValue(2000);
sheet.Cells["B4"].PutValue(3000);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the first series and set texture for a point
ChartPoint point = chart.NSeries[0].Points[2];
point.Area.FillFormat.Texture = TextureType.Stationery;
// Save the workbook
workbook.Save("TextureTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
