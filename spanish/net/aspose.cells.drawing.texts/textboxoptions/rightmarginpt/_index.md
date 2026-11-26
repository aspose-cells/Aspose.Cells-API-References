---
title: "TextBoxOptions.RightMarginPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Obtiene y establece el margen derecho en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/rightmarginpt/
---
## TextBoxOptions.RightMarginPt property

Obtiene y establece el margen derecho en unidades de Puntos.

```csharp
public double RightMarginPt { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            int textBoxIndex = worksheet.TextBoxes.Add(1, 1, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "Sample Text";

            // Establecer el margen derecho en puntos
            textBox.TextBoxOptions.RightMarginPt = 0.2d;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxRightMarginDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


