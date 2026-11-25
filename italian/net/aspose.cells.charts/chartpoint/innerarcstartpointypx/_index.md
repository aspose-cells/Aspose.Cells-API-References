---
title: "ChartPoint.InnerArcStartPointYPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata y del punto di partenza della sezione della torta dopo le chiamate al metodo Chart.Calculate. Si applica al grafico a ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/innerarcstartpointypx/
---
## ChartPoint.InnerArcStartPointYPx property

Restituisce la coordinata y del punto di partenza per la sezione della pie dopo le chiamate al metodo Chart.Calculate(). Si applica al grafico Doughnut.

```csharp
public float InnerArcStartPointYPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointYPxDemo
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
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che le proprietà siano popolate
            chart.Calculate();

            // Ottieni il primo punto del grafico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore di InnerArcStartPointYPx
            Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);

            // Nota: InnerArcStartPointYPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare la posizione, dobbiamo regolare le dimensioni del foro della ciambella
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Ricalcola il grafico per aggiornare le proprietà
            chart.Calculate();

            // Visualizza il nuovo valore di InnerArcStartPointYPx dopo aver modificato le dimensioni del foro
            Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


