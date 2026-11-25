---
title: "ChartPoint.ShapeHeightPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene l'altezza in unità di pixel dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapeheightpx/
---
## ChartPoint.ShapeHeightPx property

Ottiene l'altezza in unità di pixel dopo le chiamate al metodo Chart.Calculate().

```csharp
public int ShapeHeightPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightPxDemo
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

            // Calcola il grafico per ottenere le dimensioni della forma
            chart.Calculate();

            // Ottieni il primo punto del grafico dalla prima serie
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Visualizza l'altezza corrente della forma del punto del grafico in pixel
            Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);

            // Nota: ShapeHeightPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare l'altezza, dovremmo modificare le dimensioni del grafico o i valori dei dati
            // e ricalcolare il grafico

            // Modifica il valore dei dati che influenzerà la dimensione del punto del grafico
            worksheet.Cells["B2"].PutValue(50);
            chart.Calculate();

            // Visualizza la nuova altezza dopo aver modificato i dati
            Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);

            // Salva la cartella di lavoro
            workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


