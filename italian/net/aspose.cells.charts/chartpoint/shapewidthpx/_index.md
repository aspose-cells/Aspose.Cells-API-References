---
title: "ChartPoint.ShapeWidthPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Restituisce la larghezza in unità di pixel dopo aver chiamato il metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapewidthpx/
---
## ChartPoint.ShapeWidthPx property

Ottiene la larghezza in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

```csharp
public int ShapeWidthPx { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthPxDemo
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

            // Calcola il grafico per garantire che le proprietà della forma siano disponibili
            chart.Calculate();

            // Ottieni il primo punto del grafico dalla prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visualizza la larghezza corrente della forma del punto del grafico in pixel
            Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);

            // Nota: ShapeWidthPx è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare la larghezza, è necessario modificare le dimensioni del grafico o altre proprietà
            // ciò influirebbe sulla larghezza del punto durante il prossimo Calculate()

            // Modifica la larghezza del grafico per dimostrare come influisce su ShapeWidthPx
            chart.ChartObject.Width = 1000;
            chart.Calculate();

            // Visualizza la nuova larghezza dopo il ridimensionamento del grafico
            Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);

            // Salva il risultato
            workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


