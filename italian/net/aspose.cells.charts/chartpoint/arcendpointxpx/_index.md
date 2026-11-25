---
title: "ChartPoint.ArcEndPointXPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata x del punto finale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate. Si applica ai grafici a torta e a ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/arcendpointxpx/
---
## ChartPoint.ArcEndPointXPx property

Ottiene la coordinata x del punto finale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a torta e ciambella.

```csharp
public float ArcEndPointXPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointXPxDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che le proprietà siano popolate
            chart.Calculate();

            // Ottieni il primo punto del grafico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostra il valore di ArcEndPointXPx
            Console.WriteLine("ArcEndPointXPx: " + point.ArcEndPointXPx);

            // Nota: ArcEndPointXPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare il punto finale, dobbiamo modificare i dati del grafico o le proprietà che influenzano la fetta di torta
            
            // Esempio di come la modifica dei dati influisce su ArcEndPointXPx
            worksheet.Cells["B2"].PutValue(60); // Increase Apple's value
            chart.Calculate(); // Recalculate chart

            // Mostra il nuovo valore di ArcEndPointXPx dopo la modifica dei dati
            Console.WriteLine("New ArcEndPointXPx after data change: " + point.ArcEndPointXPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


