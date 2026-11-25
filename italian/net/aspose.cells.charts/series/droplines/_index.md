---
title: "Series.DropLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce un oggetto Line che rappresenta le linee di discesa per una serie nel grafico a linee o nel grafico ad area. Si applica solo ai grafici a linee o ad area"
type: docs
url: /it/net/aspose.cells.charts/series/droplines/
---
## Series.DropLines property

Restituisce un oggetto [`Line`](../../../aspose.cells.drawing/line/) che rappresenta le linee di discesa per una serie nel grafico a linee o nel grafico ad area. Si applica solo ai grafici a linee o ad area.

```csharp
public Line DropLines { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyDropLinesDemo
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

            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["B5"].PutValue(210);

            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(130);
            worksheet.Cells["C4"].PutValue(160);
            worksheet.Cells["C5"].PutValue(190);

            // Aggiungi un grafico a linee
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Abilita le linee di discesa per il grafico
            chart.NSeries[0].HasDropLines = true;
            chart.NSeries[1].HasDropLines = true;

            // Accedi alle linee di discesa per la prima serie
            Line dropLines = chart.NSeries[0].DropLines;

            // Visualizza le proprietà attuali delle linee di discesa
            Console.WriteLine("Drop line color: " + dropLines.Color);
            Console.WriteLine("Drop line style: " + dropLines.Style);
            Console.WriteLine("Drop line weight: " + dropLines.Weight);

            // Modifica le proprietà delle linee di discesa
            dropLines.Color = System.Drawing.Color.Red;
            dropLines.Style = LineType.Solid;
            dropLines.Weight = WeightType.MediumLine;
            dropLines.DashType = MsoLineDashStyle.Solid;
            dropLines.IsVisible = true;

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyDropLinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


