---
title: "PlotArea.SetPositionAuto"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PlotArea. Imposta la posizione dell'area del grafico su automatico"
type: docs
url: /it/net/aspose.cells.charts/plotarea/setpositionauto/
---
## PlotArea.SetPositionAuto method

Imposta la posizione dell'area del grafico su automatico

```csharp
public override void SetPositionAuto()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaMethodSetPositionAutoDemo
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

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Ottieni l'area del grafico
                PlotArea plotArea = chart.PlotArea;
                
                // Imposta manualmente alcuni valori di posizione prima per dimostrare l'effetto
                plotArea.XRatioToChart = 0.1;
                plotArea.YRatioToChart = 0.1;
                plotArea.WidthRatioToChart = 0.8;
                plotArea.HeightRatioToChart = 0.8;
                
                // Chiama SetPositionAuto per ripristinare il posizionamento automatico
                plotArea.SetPositionAuto();
                
                Console.WriteLine("Plot area position has been set to automatic.");
                
                // Salva la cartella di lavoro per mostrare l'effetto
                workbook.Save("PlotAreaSetPositionAutoDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


