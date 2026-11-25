---
title: "Legend.GetLegendLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Legend. Ottiene le etichette delle voci della legenda dopo la chiamata al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/legend/getlegendlabels/
---
## Legend.GetLegendLabels method

Ottiene le etichette delle voci della legenda dopo la chiamata al metodo Chart.Calculate().

```csharp
public string[] GetLegendLabels()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendMethodGetLegendLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calcola il grafico
            chart.Calculate();
            
            // Ottieni le etichette della legenda
            string[] legendLabels = chart.Legend.GetLegendLabels();
            
            // Visualizza le etichette della legenda
            Console.WriteLine("Legend Labels:");
            foreach (string label in legendLabels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### Vedi anche

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


