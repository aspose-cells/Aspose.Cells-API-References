---
title: "DataLabels.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Ottiene o imposta il testo dell'etichetta dati"
type: docs
url: /it/net/aspose.cells.charts/datalabels/text/
---
## DataLabels.Text property

Ottiene o imposta il testo dell'etichetta dati.

```csharp
public override string Text { get; set; }
```

### Osservazioni

Funziona solo quando si tratta di un'etichetta dati di un punto del grafico.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["A4"].PutValue("Product C");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita le etichette dei dati
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Aspose.Cells.Charts.Series series = chart.NSeries[i];
                series.DataLabels.ShowValue = true;
                
                // Personalizza il testo dell'etichetta dati
                for (int j = 0; j < series.Points.Count; j++)
                {
                    series.Points[j].DataLabels.Text = $"+{series.Points[j].YValue}";
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsTextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


