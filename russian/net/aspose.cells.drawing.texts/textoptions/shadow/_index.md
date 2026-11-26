---
title: "TextOptions.Shadow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Представляет объект ShadowEffect, который задает эффект тени для элемента диаграммы или фигуры"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/shadow/
---
## TextOptions.Shadow property

Представляет объект [`ShadowEffect`](../../../aspose.cells.drawing/shadoweffect/), который задает эффект тени для элемента диаграммы или фигуры.

```csharp
public ShadowEffect Shadow { get; }
```

### Примеры

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

### См. также

* class [ShadowEffect](../../../aspose.cells.drawing/shadoweffect/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


