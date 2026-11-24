---
title: "SvgImageOptions.CssPrefix"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SvgImageOptions Eigenschaft. Gibt den Präfix des CSS-Namens im SVG zurück und setzt ihn. Der Standardwert ist ein leerer String"
type: docs
url: /de/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

Ermittelt und legt das Präfix des CSS-Namens in SVG fest, der Standardwert ist eine leere Zeichenkette.

```csharp
public string CssPrefix { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
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

            // Erstelle ein Liniendiagramm
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // Erstelle SVG-Bildoptionen
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Zeige den aktuellen CSS-Präfix an
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // Setze neuen CSS-Präfix
            svgOptions.CssPrefix = "chart-prefix-";

            // Demonstriere die SVG-Erzeugung mit benutzerdefiniertem CSS-Präfix
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### Siehe auch

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


