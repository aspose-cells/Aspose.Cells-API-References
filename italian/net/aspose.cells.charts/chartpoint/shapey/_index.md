---
title: "ChartPoint.ShapeY"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'altezza del grafico dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapey/
---
## ChartPoint.ShapeY property

Ottiene la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'altezza del grafico dopo le chiamate al metodo Chart.Calculate().

```csharp
public int ShapeY { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYDemo
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

            // Visualizza il valore corrente di ShapeY (1/4000 dell'altezza del grafico)
            Console.WriteLine("Current ShapeY value: " + point.ShapeY);

            // Nota: ShapeY è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare la posizione, dovremmo modificare i dati sottostanti o le proprietà del grafico

            // Dimostra come ShapeY si relaziona alla posizione reale
            Console.WriteLine("ShapeY in pixels: " + point.ShapeYPx);
            Console.WriteLine("Chart height in pixels: " + (point.ShapeYPx * 4000 / point.ShapeY));

            // Salva il risultato
            workbook.Save("ChartPointPropertyShapeYDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


