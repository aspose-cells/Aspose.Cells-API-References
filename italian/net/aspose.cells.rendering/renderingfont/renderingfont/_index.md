---
title: "RenderingFont.RenderingFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore RenderingFont. Inizializza una nuova istanza di RenderingFont"
type: docs
url: /it/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

Inizializza una nuova istanza di [`RenderingFont`](../)

```csharp
public RenderingFont(string fontName, float fontSize)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontName | String | nome del font |
| fontSize | Single | dimensione del carattere in punti |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un carattere usando il costruttore #ctor(string, single)
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // Crea lo stile e imposta il carattere
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // Applica lo stile alla cella
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


