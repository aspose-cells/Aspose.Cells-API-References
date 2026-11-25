---
title: "ChartFrame.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta la larghezza del frame in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Ottiene o imposta la larghezza del frame in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Osservazioni

Come convertire le unità di 1/4000 in pixel? Larghezza in pixel = Larghezza * Chart.ChartObject.Height / 4000d;

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.WidthRatioToChart, invece. Width = WidthRatioToChart * 4000; Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico e ottieni il suo frame del grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            ChartFrame chartFrame = chart.ChartArea;

            // Imposta e visualizza la larghezza originale
            chartFrame.Width = 800;
            Console.WriteLine("Original Width: " + chartFrame.Width);

            // Modifica la larghezza
            chartFrame.Width = 1000;
            Console.WriteLine("Modified Width: " + chartFrame.Width);

            // Salva la cartella di lavoro
            workbook.Save("ChartFrameWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


