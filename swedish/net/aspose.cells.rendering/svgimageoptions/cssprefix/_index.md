---
title: "SvgImageOptions.CssPrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SvgImageOptions-egenskap. Hämtar och anger prefixet för css-namnet i svg. Standardvärdet är en tom sträng"
type: docs
url: /sv/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

Hämtar och anger prefixet för css-namnet i svg, standardvärdet är en tom sträng.

```csharp
public string CssPrefix { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyCssPrefixDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue(2019);
            worksheet.Cells["A3"].PutValue(2020);
            worksheet.Cells["A4"].PutValue(2021);
            worksheet.Cells["A5"].PutValue(2022);

            worksheet.Cells["B2"].PutValue(4500);
            worksheet.Cells["B3"].PutValue(4900);
            worksheet.Cells["B4"].PutValue(5200);
            worksheet.Cells["B5"].PutValue(6100);

            // Skapa ett linjediagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // Skapa SVG-bildalternativ
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Visa aktuellt CSS-prefix
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // Ange nytt CSS-prefix
            svgOptions.CssPrefix = "chart-prefix-";

            // Demonstrera SVG-generering med anpassat CSS-prefix
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### Se även

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


