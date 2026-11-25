---
title: "ChartFrame.SetPositionAuto"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartFrame. Imposta la posizione del frame su automatico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/setpositionauto/
---
## ChartFrame.SetPositionAuto method

Imposta la posizione del frame su automatico

```csharp
public virtual void SetPositionAuto()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFrameMethodSetPositionAutoDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni il frame del titolo del grafico
            ChartFrame title = chart.Title;
            
            // Imposta prima la posizione manuale per dimostrare SetPositionAuto
            title.XRatioToChart = 0.2;
            title.YRatioToChart = 0.1;
            title.WidthRatioToChart = 0.6;
            title.HeightRatioToChart = 0.1;

            try
            {
                // Chiama il metodo SetPositionAuto
                title.SetPositionAuto();
                
                Console.WriteLine("Chart title position set to automatic successfully");
                
                // Visualizza i nuovi valori di posizione automatica
                Console.WriteLine($"New X position ratio: {title.XRatioToChart}");
                Console.WriteLine($"New Y position ratio: {title.YRatioToChart}");
                Console.WriteLine($"New Width ratio: {title.WidthRatioToChart}");
                Console.WriteLine($"New Height ratio: {title.HeightRatioToChart}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("ChartFrameSetPositionAutoDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


