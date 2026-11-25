---
title: "ChartPoint.ShapeHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene l'altezza in unità di 1/4000 dell'altezza del grafico dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapeheight/
---
## ChartPoint.ShapeHeight property

Ottiene l'altezza in unità di 1/4000 dell'altezza del grafico dopo le chiamate al metodo Chart.Calculate().

```csharp
public int ShapeHeight { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightDemo
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
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che le proprietà della forma siano disponibili
            chart.Calculate();

            // Ottieni il primo punto nella prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza il valore corrente di ShapeHeight (in 1/4000 dell'altezza del grafico)
            Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);

            // Nota: ShapeHeight è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare l'altezza, è necessario modificare le dimensioni del grafico o altre proprietà

            // Dimostra l'effetto modificando l'altezza del grafico
            Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
            chart.ChartObject.Height = 400;
            chart.Calculate(); // Recalculate to update shape properties

            // Visualizza il nuovo valore di ShapeHeight dopo aver modificato l'altezza del grafico
            Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);

            // Salva il risultato
            workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


