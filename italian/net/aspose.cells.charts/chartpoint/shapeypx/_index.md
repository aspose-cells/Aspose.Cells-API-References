---
title: "ChartPoint.ShapeYPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata y dell'angolo superiore sinistro in unità di pixel dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapeypx/
---
## ChartPoint.ShapeYPx property

Ottiene la coordinata y dell'angolo in alto a sinistra in unità di pixel dopo le chiamate al metodo Chart.Calculate().

```csharp
public int ShapeYPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYPxDemo
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

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per ottenere le posizioni delle forme
            chart.Calculate();

            // Ottieni il primo punto nella prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza la posizione Y corrente in pixel
            Console.WriteLine("Current ShapeYPx value: " + point.ShapeYPx);

            // Nota: ShapeYPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per cambiare la posizione, dobbiamo modificare la dimensione/posizione del grafico o i dati

            // Dimostra l'effetto cambiando la posizione del grafico, il che influenzerà le posizioni dei punti
            chart.Move(2, 3, 17, 11); // Move chart to row 2, column 3
            chart.Calculate(); // Recalculate to update positions

            // Mostra la nuova posizione Y dopo lo spostamento del grafico
            Console.WriteLine("New ShapeYPx value after chart movement: " + point.ShapeYPx);

            // Salva il risultato
            workbook.Save("ChartPointShapeYPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


