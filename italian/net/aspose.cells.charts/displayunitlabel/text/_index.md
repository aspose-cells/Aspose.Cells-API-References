---
title: "DisplayUnitLabel.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DisplayUnitLabel. Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione"
type: docs
url: /it/net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione.

```csharp
public override string Text { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A1:A4", true);
            
            // Configura l'etichetta dell'unità di visualizzazione
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Accedi e modifica il testo dell'etichetta dell'unità di visualizzazione
            DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
            Console.WriteLine("Default Display Unit Label: " + label.Text);
            
            // Modifica il testo
            label.Text = "K Units";
            Console.WriteLine("Modified Display Unit Label: " + label.Text);
            
            // Salva la cartella di lavoro
            workbook.Save("DisplayUnitLabelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


