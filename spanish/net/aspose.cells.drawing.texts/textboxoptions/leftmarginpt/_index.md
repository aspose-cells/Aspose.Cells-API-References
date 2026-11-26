---
title: "TextBoxOptions.LeftMarginPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Obtiene y establece el margen izquierdo en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/leftmarginpt/
---
## TextBoxOptions.LeftMarginPt property

Obtiene y establece el margen izquierdo en unidades de Puntos.

```csharp
public double LeftMarginPt { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyLeftMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 400);
            textBox.TextBoxOptions.LeftMarginPt = 0.2d;

            Console.WriteLine("Left margin set to: " + textBox.TextBoxOptions.LeftMarginPt + " points");
        }
    }
}
```

### Ver también

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


