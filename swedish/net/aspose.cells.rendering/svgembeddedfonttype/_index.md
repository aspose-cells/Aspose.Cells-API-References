---
title: "Enum SvgEmbeddedFontType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.SvgEmbeddedFontType enum. Representerar den inbäddade typsnittstypen i en Svg-bild"
type: docs
url: /sv/net/aspose.cells.rendering/svgembeddedfonttype/
---
## SvgEmbeddedFontType enumeration

Representerar den inbäddade teckensnittstypen i en SVG-bild.

```csharp
public enum SvgEmbeddedFontType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Inte inbädda typsnitt. |
| Woff | `1` | Inbädda WOFF-typsnitt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Konfigurera SVG-bildalternativ
            SvgImageOptions svgOptions = new SvgImageOptions
            {
                EmbeddedFontType = SvgEmbeddedFontType.Woff,
                FitToViewPort = true,
                CssPrefix = "chart-prefix"
            };

            // Spara diagrammet som SVG med inbäddat WOFF-typsnitt
            chart.ToImage("output_chart.svg", svgOptions);

            Console.WriteLine("SVG with embedded WOFF font generated successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


