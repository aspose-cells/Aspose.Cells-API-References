---
title: ShapeCollection.AddTextEffectInChart
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Inserts a WordArt object to the chart
type: docs
url: /net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
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
// Called: Shape wordart = chart.Shapes.AddTextEffectInChart(MsoPresetTextEffect.TextEffect2,
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ReportTest.xls");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Shape wordart = chart.Shapes.AddTextEffectInChart(MsoPresetTextEffect.TextEffect2,
                "CONFIDENTIAL", "Arial Black", 66, false, false
                 , 1200, 500, 2000, 3000);
            MsoFillFormat wordArtFormat = wordart.FillFormat;
            //fillFormat.ForeColor = System.Drawing.Color.Black;
            wordArtFormat.Transparency = 0.9;
            MsoLineFormat lineFormat = wordart.LineFormat;
            lineFormat.IsVisible = false;
            workbook.Save(Constants.destPath + "Test_WordArt.xls");
        }
```

### See Also

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


