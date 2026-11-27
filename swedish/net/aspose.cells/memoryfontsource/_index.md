---
title: "Klass MemoryFontSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.MemoryFontSource-klass. Representerar den enda TrueType-typsnittsfilen som lagras i minnet."
type: docs
url: /sv/net/aspose.cells/memoryfontsource/
---
## MemoryFontSource class

Representerar den enskilda TrueType-typsnittsfilen som lagras i minnet.

```csharp
public class MemoryFontSource : FontSourceBase
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | Konstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | Binär typsnittsdata. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | Returnerar typen av teckensnittskälla. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassMemoryFontSourceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Läs in en TrueType-typsnittfil i minnet
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Skapa en instans av MemoryFontSource med typsnittsdata
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Skapa en array av typsnittskällor som innehåller vår MemoryFontSource
            FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };

            // Ställ in typsnittskällorna med hjälp av FontConfigs
            FontConfigs.SetFontSources(fontSources);

            // Använd det anpassade typsnittet i en cell
            worksheet.Cells["A1"].PutValue("Text with custom font from memory");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);

            // Spara arbetsboken
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


