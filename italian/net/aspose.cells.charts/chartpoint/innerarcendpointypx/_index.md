---
title: "ChartPoint.InnerArcEndPointYPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata y del punto finale della sezione della torta dopo le chiamate al metodo Chart.Calculate. Si applica al grafico a ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/innerarcendpointypx/
---
## ChartPoint.InnerArcEndPointYPx property

Ottiene la coordinata y del punto finale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico a ciambella.

```csharp
public float InnerArcEndPointYPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(25);

            // Aggiungi un grafico a ciambella
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per ottenere le proprietà dei punti del grafico
            chart.Calculate();

            // Ottieni il primo punto del grafico dalla prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore corrente di InnerArcEndPointYPx
            Console.WriteLine("Current InnerArcEndPointYPx value: " + point.InnerArcEndPointYPx);

            // Nota: InnerArcEndPointYPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare la posizione, dobbiamo modificare le dimensioni del foro della ciambella
            chart.NSeries[0].DoughnutHoleSize = 60; // Change hole size to affect inner arc position

            // Ricalcola il grafico per aggiornare le proprietà
            chart.Calculate();

            // Visualizza il nuovo valore di InnerArcEndPointYPx dopo aver modificato le dimensioni del foro
            Console.WriteLine("New InnerArcEndPointYPx value after changing hole size: " + point.InnerArcEndPointYPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyInnerArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


