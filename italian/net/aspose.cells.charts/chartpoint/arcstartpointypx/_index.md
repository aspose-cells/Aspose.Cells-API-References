---
title: "ChartPoint.ArcStartPointYPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ChartPoint property. Restituisce la coordinata y del punto di partenza per la sezione a torta dopo le chiamate al metodo Chart.Calculate. Si applica ai grafici a torta e ciambella"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/arcstartpointypx/
---
## ChartPoint.ArcStartPointYPx property

Ottiene la coordinata y del punto iniziale per la sezione a torta dopo aver chiamato il metodo Chart.Calculate(). Si applica ai grafici a torta e ciambella.

```csharp
public float ArcStartPointYPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointYPxDemo
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

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per ottenere le posizioni delle forme
            chart.Calculate();

            // Ottieni il primo punto del grafico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore corrente di ArcStartPointYPx
            Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);

            // Nota: ArcStartPointYPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Invece, dimostreremo come la modifica di altre proprietà influisce su ArcStartPointYPx

            // Modifica il valore di esplosione per modificare la posizione della fetta di torta
            point.Explosion = 20;

            // Ricalcola il grafico per aggiornare le posizioni
            chart.Calculate();

            // Visualizza il nuovo valore di ArcStartPointYPx dopo aver modificato l'esplosione
            Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


