---
title: "TextBoxOptions.BottomMarginPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Devuelve el margen inferior en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/bottommarginpt/
---
## TextBoxOptions.BottomMarginPt property

Devuelve el margen inferior en unidades de puntos

```csharp
public double BottomMarginPt { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyBottomMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.TextBoxOptions.BottomMarginPt = 0.2d;

            Console.WriteLine("Bottom margin set to: " + shape.TextBoxOptions.BottomMarginPt + " points");
        }
    }
}
```

### Ver también

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


