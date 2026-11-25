---
title: "ChartPoint.GetOnCategoryAxisPointYPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartPoint. Ottiene la coordinata y del punto sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate. Si applica solo al grafico ad area"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/getoncategoryaxispointypx/
---
## ChartPoint.GetOnCategoryAxisPointYPx method

Ottiene la coordinata y del punto sull'asse delle categorie dopo aver chiamato il metodo Chart.Calculate(). Si applica solo ai grafici Area.

```csharp
public float GetOnCategoryAxisPointYPx(int index)
```

### Osservazioni

Grafico Area 2D: l'indice è 0. Grafico Area 3D: l'indice è 0 o 1.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointYPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che tutte le proprietà di posizione siano calcolate
            chart.Calculate();

            // Ottieni il primo punto del grafico dalla prima serie
            ChartPoint point = chart.NSeries[0].Points[0];

            try
            {
                // Chiama GetOnCategoryAxisPointYPx con indice 0
                float yPx = point.GetOnCategoryAxisPointYPx(0);
                
                // Visualizza il risultato
                Console.WriteLine($"Y coordinate of point on category axis: {yPx} pixels");
                
                // Salva la cartella di lavoro
                workbook.Save("ChartPointGetOnCategoryAxisPointYPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointYPx method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


