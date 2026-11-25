---
title: "ChartPoint.InnerArcStartPointXPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata x del punto di partenza per la sezione a torta dopo aver chiamato il metodo Chart.Calculate. Si applica al grafico a ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/innerarcstartpointxpx/
---
## ChartPoint.InnerArcStartPointXPx property

Ottiene la coordinata x del punto iniziale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica al grafico a ciambella.

```csharp
public float InnerArcStartPointXPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointXPxDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a ciambella
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per ottenere le proprietà della forma
            chart.Calculate();

            // Ottieni il primo punto del grafico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore di InnerArcStartPointXPx
            Console.WriteLine("InnerArcStartPointXPx: " + point.InnerArcStartPointXPx);

            // Nota: InnerArcStartPointXPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare la posizione, dovremmo modificare le dimensioni del grafico o la dimensione del foro della ciambella

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyInnerArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


