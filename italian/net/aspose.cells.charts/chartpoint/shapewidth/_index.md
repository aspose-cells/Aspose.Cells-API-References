---
title: "ChartPoint.ShapeWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene la larghezza in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapewidth/
---
## ChartPoint.ShapeWidth property

Ottiene la larghezza in unità di 1/4000 della larghezza del grafico dopo aver chiamato il metodo Chart.Calculate().

```csharp
public int ShapeWidth { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthDemo
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
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calcola il grafico per garantire che le proprietà della forma siano disponibili
            chart.Calculate();
            
            // Ottieni il primo punto del grafico nella prima serie
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Visualizza il valore corrente di ShapeWidth (in 1/4000 della larghezza del grafico)
            Console.WriteLine("Current ShapeWidth value: " + point.ShapeWidth);
            
            // Visualizza la larghezza in pixel
            Console.WriteLine("Shape width in pixels: " + point.ShapeWidthPx);
            
            // Nota: ShapeWidth è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per modificare la larghezza, sarebbe necessario modificare le dimensioni del grafico o altre proprietà
            
            // Salva il risultato
            workbook.Save("ChartPointShapeWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


