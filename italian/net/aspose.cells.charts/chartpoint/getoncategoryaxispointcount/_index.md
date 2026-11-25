---
title: "ChartPoint.GetOnCategoryAxisPointCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartPoint. Ottiene il numero di punti sull'asse delle categorie dopo la chiamata al metodo Chart.Calculate. Si applica solo ai grafici ad area"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/getoncategoryaxispointcount/
---
## ChartPoint.GetOnCategoryAxisPointCount method

Ottiene il numero di punti sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate(). Si applica solo ai grafici area.

```csharp
public int GetOnCategoryAxisPointCount()
```

### Osservazioni

Il grafico ad area 2D restituisce 1, il grafico ad area 3D restituisce 2.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointCountDemo
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

            // Aggiungi un grafico ad area
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che tutti i punti del grafico siano calcolati
            chart.Calculate();

            try
            {
                // Ottieni il primo punto del grafico dalla prima serie
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Chiama il metodo GetOnCategoryAxisPointCount
                int pointCount = point.GetOnCategoryAxisPointCount();
                
                Console.WriteLine($"Number of points on category axis: {pointCount}");
                
                // Visualizza le coordinate di ciascun punto sull'asse delle categorie
                for (int i = 0; i < pointCount; i++)
                {
                    float x = point.GetOnCategoryAxisPointXPx(i);
                    float y = point.GetOnCategoryAxisPointYPx(i);
                    Console.WriteLine($"Point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointCount method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("MethodGetOnCategoryAxisPointCountDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


