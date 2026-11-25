---
title: "SvgImageOptions.SvgImageOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore SvgImageOptions. Ctor"
type: docs
url: /it/net/aspose.cells.rendering/svgimageoptions/svgimageoptions/
---
## SvgImageOptions constructor

Ctor.

```csharp
public SvgImageOptions()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Month");
            worksheet.Cells["A2"].PutValue("Jan");
            worksheet.Cells["A3"].PutValue("Feb");
            worksheet.Cells["A4"].PutValue("Mar");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(210);
            worksheet.Cells["B4"].PutValue(150);

            // Crea un grafico a linee
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Crea SvgImageOptions usando il costruttore
                SvgImageOptions svgOptions = new SvgImageOptions();

                // Configura le opzioni di rendering SVG
                svgOptions.ImageType = ImageType.Svg; // Explicitly set to SVG
                svgOptions.FitToViewPort = true;
                svgOptions.CssPrefix = "chart-prefix";
                svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

                // Salva il grafico come SVG con le opzioni specificate
                chart.ToImage("output_chart.svg", svgOptions);

                Console.WriteLine("SVG image saved successfully with specified options.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error generating SVG: {ex.Message}");
            }

            // Salva la cartella di lavoro per dimostrare i dati originali
            workbook.Save("SvgImageOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


