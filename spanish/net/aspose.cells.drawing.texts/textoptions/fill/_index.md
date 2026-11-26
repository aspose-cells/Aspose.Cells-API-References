---
title: "TextOptions.Fill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Representa el formato de relleno del texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

Representa el formato de relleno del texto.

```csharp
public FillFormat Fill { get; }
```

### Ejemplos

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
            
            // Establecer propiedades de fuente
            textOptions.Name = "Arial";
            textOptions.Size = 14;
            textOptions.IsBold = true;
            
            // Demostrar la propiedad Fill
            textOptions.Fill.FillType = FillType.Solid;
            SolidFill solidFill = textOptions.Fill.SolidFill;
            solidFill.Color = System.Drawing.Color.Blue;
            
            // Guarda el libro de trabajo
            workbook.Save("TextOptionsFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


