---
title: TextOptions.Fill
second_title: Aspose.Cells for .NET API Reference
description: TextOptions property. Represents the fill format of the text
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

Represents the fill format of the text.

```csharp
public FillFormat Fill { get; }
```

### Examples

```csharp
// Called: SolidFill fill = font.Fill.SolidFill;
public void TextOptions_Property_Fill()
{

    Workbook workbook = new Workbook();
    Worksheet sheet = workbook.Worksheets[0];
    Shape sp = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 4, 4, 4, 4, 100, 700);
    sp.Fill.FillType = FillType.None;

    sp.Text = "Hello World !!!";
    FontSetting fs = sp.Characters(0, "Hello World !!!".Length);
    TextOptions font = fs.TextOptions;
    font.Name = "Calibri";
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

    Util.SaveManCheck(workbook, "Shape", "example.xlsx");
}
```

### See Also

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


