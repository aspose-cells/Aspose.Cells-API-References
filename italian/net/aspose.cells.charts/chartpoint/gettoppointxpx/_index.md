---
title: "ChartPoint.GetTopPointXPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartPoint. Restituisce la coordinata x del punto superiore della forma dopo le chiamate al metodo Chart.Calculate. Si applica ai grafici 3D Column3D, Bar3D, Cone, Cylinder, Pyramid e Area3D"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/gettoppointxpx/
---
## ChartPoint.GetTopPointXPx method

Ottiene la coordinata x del punto superiore della forma dopo le chiamate al metodo Chart.Calculate(). Si applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid e Area3D

```csharp
public float GetTopPointXPx(int index)
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointXPxWithInt32Demo
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che tutte le proprietà di posizione siano calcolate
            chart.Calculate();

            try
            {
                // Ottieni il primo punto del grafico dalla prima serie
                ChartPoint point = chart.NSeries[0].Points[0];

                // Ottieni il numero di punti superiori
                int pointCount = point.GetTopPointCount();

                if (pointCount > 0)
                {
                    // Chiama GetTopPointXPx con indice 0
                    float xPos = point.GetTopPointXPx(0);
                    Console.WriteLine($"X position of top point (pixels): {xPos}");
                }
                else
                {
                    Console.WriteLine("No top points available for this chart point");
                }

                Console.WriteLine("Method executed successfully with parameters (Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointXPx method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("ChartPointMethodGetTopPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


