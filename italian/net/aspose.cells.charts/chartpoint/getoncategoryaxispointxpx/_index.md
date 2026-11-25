---
title: "ChartPoint.GetOnCategoryAxisPointXPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartPoint. Ottiene la coordinata x del punto sull'asse di categoria dopo le chiamate al metodo Chart.Calculate. Si applica solo ai grafici Area chart"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/getoncategoryaxispointxpx/
---
## ChartPoint.GetOnCategoryAxisPointXPx method

Ottiene la coordinata x del punto sull'asse delle categorie dopo le chiamate al metodo Chart.Calculate(). Si applica solo al grafico Area.

```csharp
public float GetOnCategoryAxisPointXPx(int index)
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

    public class ChartPointMethodGetOnCategoryAxisPointXPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico
            chart.Calculate();

            try
            {
                // Ottieni il primo punto del grafico
                ChartPoint point = chart.NSeries[0].Points[0];

                // Chiama GetOnCategoryAxisPointXPx con indice 0
                float xPosition = point.GetOnCategoryAxisPointXPx(0);

                // Visualizza il risultato
                Console.WriteLine($"X position of first category axis point: {xPosition} pixels");

                // Salva la cartella di lavoro
                workbook.Save("ChartPointGetOnCategoryAxisPointXPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointXPx method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


