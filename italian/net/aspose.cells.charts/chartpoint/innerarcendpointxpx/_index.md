---
title: "ChartPoint.InnerArcEndPointXPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata x del punto finale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate. Si applica ai grafici a ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/innerarcendpointxpx/
---
## ChartPoint.InnerArcEndPointXPx property

Ottiene la coordinata x del punto finale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a ciambella.

```csharp
public float InnerArcEndPointXPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(2);

            // Aggiungi un grafico a ciambella
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per ottenere le proprietà dei punti del grafico
            chart.Calculate();

            // Ottieni il primo punto del grafico dalla prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostra il valore corrente di InnerArcEndPointXPx
            Console.WriteLine("Current InnerArcEndPointXPx value: " + point.InnerArcEndPointXPx);

            // Nota: InnerArcEndPointXPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare la posizione del punto finale, dobbiamo modificare la dimensione del foro della ciambella
            chart.NSeries[0].DoughnutHoleSize = 50; // Set hole size to 50%

            // Ricalcola il grafico per aggiornare le proprietà
            chart.Calculate();

            // Mostra il nuovo valore di InnerArcEndPointXPx dopo aver modificato la dimensione del foro
            Console.WriteLine("New InnerArcEndPointXPx value after changing doughnut hole size: " + point.InnerArcEndPointXPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyInnerArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


