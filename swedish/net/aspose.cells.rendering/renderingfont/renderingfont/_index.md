---
title: "RenderingFont.RenderingFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingFont-konstruktor. Initierar en ny instans av RenderingFont"
type: docs
url: /sv/net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

Initierar en ny instans av [`RenderingFont`](../)

```csharp
public RenderingFont(string fontName, float fontSize)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontName | String | teckensnittsnamn |
| fontSize | Single | teckenstorlek i punkter |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett teckensnitt med #ctor(string, single)-konstruktorn
            RenderingFont font = new RenderingFont("Arial", 24f);
            font.Bold = true;
            font.Color = System.Drawing.Color.Red;
            
            // Skapa stil och ange teckensnitt
            Style style = workbook.CreateStyle();
            style.Font.Name = font.Name;
            style.Font.Size = (int)font.Size;  // Explicit cast from float to int
            style.Font.IsBold = font.Bold;
            style.Font.Color = font.Color;
            
            // Applicera stil på cell
            worksheet.Cells["A1"].PutValue("Text with custom font");
            worksheet.Cells["A1"].SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("FontDemoOutput.xlsx");
        }
    }
}
```

### Se även

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


