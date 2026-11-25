---
title: "SvgImageOptions.CssPrefix"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SvgImageOptions. Ottiene e imposta il prefisso del nome css in svg; il valore predefinito è una stringa vuota"
type: docs
url: /it/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

Ottiene e imposta il prefisso del nome CSS in SVG, il valore predefinito è una stringa vuota.

```csharp
public string CssPrefix { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
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

            // Crea un grafico a linee
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // Crea opzioni immagine SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Visualizza il prefisso CSS corrente
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // Imposta un nuovo prefisso CSS
            svgOptions.CssPrefix = "chart-prefix-";

            // Dimostra la generazione di SVG con prefisso CSS personalizzato
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### Vedi anche

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


