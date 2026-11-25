---
title: "Enum SvgEmbeddedFontType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Rendering.SvgEmbeddedFontType. Rappresenta il tipo di carattere incorporato nell'immagine Svg"
type: docs
url: /it/net/aspose.cells.rendering/svgembeddedfonttype/
---
## SvgEmbeddedFontType enumeration

Rappresenta il tipo di carattere incorporato nell'immagine SVG.

```csharp
public enum SvgEmbeddedFontType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Non incorporare il carattere. |
| Woff | `1` | Incorpora il carattere WOFF. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Configura le opzioni dell'immagine SVG
            SvgImageOptions svgOptions = new SvgImageOptions
            {
                EmbeddedFontType = SvgEmbeddedFontType.Woff,
                FitToViewPort = true,
                CssPrefix = "chart-prefix"
            };

            // Salva il grafico come SVG con font WOFF incorporato
            chart.ToImage("output_chart.svg", svgOptions);

            Console.WriteLine("SVG with embedded WOFF font generated successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


