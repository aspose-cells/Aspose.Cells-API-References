---
title: "DataLabels.ApplyFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DataLabels. Applica il carattere delle etichette dati a tutti i nodi figli"
type: docs
url: /it/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

Applica il carattere delle etichette dati a tutti i nodi figlio.

```csharp
public void ApplyFont()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Mostra etichette dati
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Imposta un nuovo colore del carattere per le etichette dati
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // Applica le impostazioni del carattere a tutte le etichette dati
            series.DataLabels.ApplyFont();
            
            // Salva la cartella di lavoro
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


