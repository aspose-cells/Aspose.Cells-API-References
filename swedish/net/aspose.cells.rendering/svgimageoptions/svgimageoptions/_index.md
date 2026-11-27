---
title: "SvgImageOptions.SvgImageOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SvgImageOptions-konstruktor. Ctor"
type: docs
url: /sv/net/aspose.cells.rendering/svgimageoptions/svgimageoptions/
---
## SvgImageOptions constructor

Konstruktor.

```csharp
public SvgImageOptions()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Month");
            worksheet.Cells["A2"].PutValue("Jan");
            worksheet.Cells["A3"].PutValue("Feb");
            worksheet.Cells["A4"].PutValue("Mar");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(210);
            worksheet.Cells["B4"].PutValue(150);

            // Skapa ett linjediagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Skapa SvgImageOptions med hjälp av konstruktorn
                SvgImageOptions svgOptions = new SvgImageOptions();

                // Konfigurera SVG‑renderingsalternativ
                svgOptions.ImageType = ImageType.Svg; // Explicitly set to SVG
                svgOptions.FitToViewPort = true;
                svgOptions.CssPrefix = "chart-prefix";
                svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

                // Spara diagrammet som SVG med angivna alternativ
                chart.ToImage("output_chart.svg", svgOptions);

                Console.WriteLine("SVG image saved successfully with specified options.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error generating SVG: {ex.Message}");
            }

            // Spara arbetsboken för att demonstrera originaldata
            workbook.Save("SvgImageOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


