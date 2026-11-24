---
title: "Aufzählung SvgEmbeddedFontType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.SvgEmbeddedFontType Enum. Stellt den eingebetteten Schriftarttyp im Svg‑Bild dar."
type: docs
url: /de/net/aspose.cells.rendering/svgembeddedfonttype/
---
## SvgEmbeddedFontType enumeration

Stellt den eingebetteten Schriftarttyp in einem SVG-Bild dar.

```csharp
public enum SvgEmbeddedFontType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Schrift nicht einbetten. |
| Woff | `1` | WOFF-Schrift einbetten. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // SVG-Bildoptionen konfigurieren
            SvgImageOptions svgOptions = new SvgImageOptions
            {
                EmbeddedFontType = SvgEmbeddedFontType.Woff,
                FitToViewPort = true,
                CssPrefix = "chart-prefix"
            };

            // Diagramm als SVG mit eingebetteter WOFF-Schrift speichern
            chart.ToImage("output_chart.svg", svgOptions);

            Console.WriteLine("SVG with embedded WOFF font generated successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


