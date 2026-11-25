---
title: "ChartPoint.GetBottomPointYPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartPoint. Ottiene la coordinata y del punto inferiore della forma dopo le chiamate al metodo Chart.Calculate. Si applica ai grafici 3D Column3D Bar3D Cone Cylinder Pyramid"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/getbottompointypx/
---
## ChartPoint.GetBottomPointYPx method

Ottiene la coordinata y del punto inferiore della forma dopo le chiamate al metodo Chart.Calculate(). Si applica ai grafici 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid.

```csharp
public float GetBottomPointYPx(int index)
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointYPxDemo
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
            
            // Aggiungi serie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calcola il grafico per garantire che tutti i punti siano calcolati
            chart.Calculate();
            
            // Ottieni il primo punto della prima serie
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Ottieni il numero di punti inferiori
                int bottomPointCount = point.GetBottomPointCount();
                
                if (bottomPointCount > 0)
                {
                    // Chiama GetBottomPointYPx con indice 0
                    float yPx = point.GetBottomPointYPx(0);
                    
                    Console.WriteLine($"Bottom point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointYPx method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodGetBottomPointYPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


