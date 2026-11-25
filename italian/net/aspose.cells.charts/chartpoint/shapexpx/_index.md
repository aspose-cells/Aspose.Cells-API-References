---
title: "ChartPoint.ShapeXPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata x dell'angolo superiore sinistro in unità di pixel dopo aver chiamato il metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapexpx/
---
## ChartPoint.ShapeXPx property

Ottiene la coordinata x dell'angolo in alto a sinistra in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

```csharp
public int ShapeXPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXPxDemo
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

            // Ottieni il primo punto del grafico dalla prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza la posizione X corrente in pixel
            Console.WriteLine("Current ShapeXPx value: " + point.ShapeXPx);

            // Nota: ShapeXPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare la posizione, sarebbe necessario modificare le dimensioni/posizione del grafico o i dati

            // Dimostra come la proprietà cambia quando modifichiamo il grafico
            Console.WriteLine("\nChanging chart position...");
            chart.ChartObject.Left = 3;
            chart.ChartObject.Top = 2;
            chart.Calculate(); // Recalculate to update positions

            Console.WriteLine("New ShapeXPx value after chart move: " + point.ShapeXPx);

            // Salva il risultato
            workbook.Save("ChartPointPropertyShapeXPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


