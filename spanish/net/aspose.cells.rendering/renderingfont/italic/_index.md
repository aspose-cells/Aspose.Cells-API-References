---
title: "RenderingFont.Italic"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingFont. Obtiene o establece la cursiva para la fuente"
type: docs
url: /es/net/aspose.cells.rendering/renderingfont/italic/
---
## RenderingFont.Italic property

Obtiene o establece cursiva para la fuente.

```csharp
public bool Italic { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyItalicDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear un RenderingFont con la propiedad Italic establecida
            RenderingFont renderingFont = new RenderingFont("Arial", 16)
            {
                Italic = true,
                Color = Color.Red
            };

            // Aplicar la fuente a la celda A1
            sheet.Cells["A1"].PutValue("Italic Text Example");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";  // Directly use the font name
            style.Font.Size = (int)renderingFont.Size;  // Explicit cast to int
            style.Font.IsItalic = renderingFont.Italic;
            style.Font.Color = renderingFont.Color;
            sheet.Cells["A1"].SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("ItalicFontExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


