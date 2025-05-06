---
title: TextOptions.Shadow
second_title: Aspose.Cells for .NET API Reference
description: TextOptions property. Represents a ShadowEffect object that specifies shadow effect for the chart element or shape
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/shadow/
---
## TextOptions.Shadow property

Represents a [`ShadowEffect`](../../../aspose.cells.drawing/shadoweffect/) object that specifies shadow effect for the chart element or shape.

```csharp
public ShadowEffect Shadow { get; }
```

### Examples

```csharp
// Called: font.Shadow.PresetType = PresetShadowType.OffsetBottom;
[Test]
        public void Property_Shadow()
        {

            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Shape sp = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 4, 4, 4, 4, 100, 700);
            sp.Fill.FillType = FillType.None;

            sp.Text = &quot;Hello World !!!&quot;;
            FontSetting fs = sp.Characters(0, &quot;Hello World !!!&quot;.Length);
            TextOptions font = fs.TextOptions;
            font.Name = &quot;Calibri&quot;;
            font.Size = 54;
            font.IsBold = true;


            font.Color = System.Drawing.Color.Green;
            font.Outline.FillType = FillType.Solid;
            SolidFill outLineFill = (SolidFill)font.Outline.SolidFill;
            outLineFill.Color = Color.White;

            font.Fill.FillType = FillType.Solid;
            SolidFill fill = font.Fill.SolidFill;
            fill.Color = Color.Green;
            font.Shadow.PresetType = PresetShadowType.OffsetBottom;

            Util.SaveManCheck(workbook, &quot;Shape&quot;, &quot;CELLSNET41817.xlsx&quot;);
        }
```

### See Also

* class [ShadowEffect](../../../aspose.cells.drawing/shadoweffect/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


