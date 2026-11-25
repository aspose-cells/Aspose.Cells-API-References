---
title: "ChartPoint.ArcStartPointXPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ChartPoint property. Restituisce la coordinata x del punto di partenza per la sezione a torta dopo aver chiamato il metodo Chart.Calculate. Si applica ai grafici a torta e ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/arcstartpointxpx/
---
## ChartPoint.ArcStartPointXPx property

Ottiene la coordinata x del punto iniziale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a torta e ciambella.

```csharp
public float ArcStartPointXPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che le proprietà siano popolate
            chart.Calculate();

            // Ottieni il primo punto del grafico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore di ArcStartPointXPx
            Console.WriteLine("ArcStartPointXPx for first point: " + point.ArcStartPointXPx);

            // Nota: ArcStartPointXPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Invece, possiamo dimostrare come cambia quando modifichiamo altre proprietà

            // Modifica il valore di esplosione che influisce sulla posizione della fetta di torta
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update properties

            // Visualizza il nuovo valore di ArcStartPointXPx dopo la modifica dell'esplosione
            Console.WriteLine("ArcStartPointXPx after explosion: " + point.ArcStartPointXPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


