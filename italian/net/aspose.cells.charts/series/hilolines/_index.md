---
title: "Series.HiLoLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce un oggetto HiLoLines che rappresenta le linee high‑low per una serie in un grafico a linee. Si applica solo ai grafici a linee"
type: docs
url: /it/net/aspose.cells.charts/series/hilolines/
---
## Series.HiLoLines property

Restituisce un oggetto HiLoLines che rappresenta le linee alto-basso per una serie in un grafico a linee. Si applica solo ai grafici a linee.

```csharp
public Line HiLoLines { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyHiLoLinesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("High");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["B5"].PutValue(110);

            worksheet.Cells["C1"].PutValue("Low");
            worksheet.Cells["C2"].PutValue(80);
            worksheet.Cells["C3"].PutValue(60);
            worksheet.Cells["C4"].PutValue(100);
            worksheet.Cells["C5"].PutValue(70);

            // Aggiungi un grafico a linee
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B1:B5", true);
            chart.NSeries.Add("C1:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Abilita HiLoLines per la prima serie
            Series series = chart.NSeries[0];
            series.HasHiLoLines = true;

            // Accedi e modifica le proprietà di HiLoLines
            Line hiLoLines = series.HiLoLines;
            Console.WriteLine("HiLoLines visibility: " + hiLoLines.IsVisible);

            // Personalizza l'aspetto di HiLoLines
            hiLoLines.Color = System.Drawing.Color.Red;
            hiLoLines.Weight = WeightType.MediumLine;
            hiLoLines.DashType = MsoLineDashStyle.DashDot;
            hiLoLines.IsVisible = true;

            // Salva il risultato
            workbook.Save("SeriesPropertyHiLoLinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


