---
title: "TextOptions.Fill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextOptions. Rappresenta il formato di riempimento del testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

Rappresenta il formato di riempimento del testo.

```csharp
public FillFormat Fill { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
            shape.Text = "Sample Text";
            
            FontSetting fontSetting = shape.Characters(0, shape.Text.Length);
            TextOptions textOptions = fontSetting.TextOptions;
            
            // Imposta le proprietà del font
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            
            // Dimostra la proprietà Fill
            textOptions.Fill.FillType = FillType.Solid;
            SolidFill solidFill = textOptions.Fill.SolidFill;
            solidFill.Color = System.Drawing.Color.Blue;
            
            // Salva la cartella di lavoro
            workbook.Save("TextOptionsFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


