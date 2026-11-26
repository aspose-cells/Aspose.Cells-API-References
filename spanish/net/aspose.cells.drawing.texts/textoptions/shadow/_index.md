---
title: "TextOptions.Shadow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Representa un objeto ShadowEffect que especifica el efecto de sombra para el elemento del gráfico o forma"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/shadow/
---
## TextOptions.Shadow property

Representa un [`ShadowEffect`](../../../aspose.cells.drawing/shadoweffect/) objeto que especifica el efecto de sombra para el elemento del gráfico o forma.

```csharp
public ShadowEffect Shadow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 4, 4, 4, 4, 100, 700);
            shape.Fill.FillType = FillType.None;
            shape.Text = "Hello World !!!";
            
            FontSetting fontSetting = shape.Characters(0, "Hello World !!!".Length);
            TextOptions textOptions = fontSetting.TextOptions;
            
            textOptions.Name = "Calibri";
            textOptions.Size = 54;
            textOptions.IsBold = true;
            textOptions.Color = Color.Green;
            
            textOptions.Outline.FillType = FillType.Solid;
            textOptions.Outline.SolidFill.Color = Color.White;
            
            textOptions.Fill.FillType = FillType.Solid;
            ((SolidFill)textOptions.Fill.SolidFill).Color = Color.Green;
            
            textOptions.Shadow.PresetType = PresetShadowType.OffsetBottom;
            
            workbook.Save("example.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ShadowEffect](../../../aspose.cells.drawing/shadoweffect/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


