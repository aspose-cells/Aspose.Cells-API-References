---
title: "ChartPoint.InnerRadiusPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene il raggio interno della fetta di ciambella in unità di pixel dopo le chiamate al metodo Chart.Calculate. Si applica al grafico ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/innerradiuspx/
---
## ChartPoint.InnerRadiusPx property

Ottiene il raggio interno della fetta di ciambella in unità di pixel dopo le chiamate al metodo Chart.Calculate(). Si applica al grafico ciambella.

```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartPoint.DoughnutInnerRadius. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerRadiusPxDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Aggiungi un grafico a ciambella
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per ottenere le proprietà dei punti del grafico
            chart.Calculate();

            // Ottieni il primo punto del grafico dalla prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore corrente del raggio interno (proprietà di sola lettura)
            Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);

            // Nota: InnerRadiusPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare il raggio interno, è necessario regolare la dimensione del foro della ciambella
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Ricalcola il grafico per aggiornare le proprietà
            chart.Calculate();

            // Visualizza il nuovo valore del raggio interno dopo aver modificato la dimensione del foro della ciambella
            Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);

            // Salva il risultato
            workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


