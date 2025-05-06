---
title: TextOptions.Name
second_title: Aspose.Cells for .NET API Reference
description: TextOptions property. Gets and sets the name of the shape
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/name/
---
## TextOptions.Name property

Gets and sets the name of the shape.

```csharp
public override string Name { get; set; }
```

### Examples

```csharp
// Called: font.Name = &amp;quot;Calibri&amp;quot;;
[Test]
        public void Property_Name()
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

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


