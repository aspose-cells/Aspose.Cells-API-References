---
title: "RenderingFont.RenderingFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor RenderingFont. Inicializa una nueva instancia de RenderingFont"
type: docs
url: /es/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

Inicializa una nueva instancia de [`RenderingFont`](../)

```csharp
public RenderingFont(string fontName, float fontSize)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontName | String | nombre de fuente |
| fontSize | Single | tamaño de fuente en puntos |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontMethodCtorWithStringSingleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una fuente usando el constructor #ctor(string, single)
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // Crea un estilo y establece la fuente
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // Aplica el estilo a la celda
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### Ver también

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


