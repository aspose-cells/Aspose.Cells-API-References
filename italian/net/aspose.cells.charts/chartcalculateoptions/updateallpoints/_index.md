---
title: "ChartCalculateOptions.UpdateAllPoints"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartCalculateOptions. Indica se aggiornare tutti i punti dati durante il calcolo del grafico. Predefinito False. Quando si desidera ottenere il valore per ciascun punto dati nel grafico, impostarlo su true. Se questo parametro è impostato su True, i nuovi punti dati possono essere generati quando il grafico viene calcolato. Questo potrebbe aumentare le dimensioni del file Excel"
type: docs
url: /it/net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Indica se aggiornare tutti i punti dati durante l'esecuzione del calcolo del grafico. Predefinito: False. Quando si desidera ottenere il valore di ciascun punto dati nel grafico in modo specifico, impostarlo su true. Se questo parametro è impostato su True, i nuovi punti dati possono essere generati quando il grafico viene calcolato. Questo potrebbe aumentare le dimensioni del file Excel.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(400);
            worksheet.Cells["C3"].PutValue(500);
            worksheet.Cells["C4"].PutValue(600);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Abilita le etichette dei dati
            foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
            }

            // Calcola il grafico con l'opzione UpdateAllPoints
            chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });

            // Emetti alcuni valori di etichette dati per dimostrare il risultato
            Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
            Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
        }
    }
}
```

### Vedi anche

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


