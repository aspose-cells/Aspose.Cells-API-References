---
title: "Series.BubbleScale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce o imposta il fattore di scala per le bolle nel gruppo di grafico specificato. Può essere un valore intero da 0 a 300 corrispondente a una percentuale della dimensione predefinita. Si applica solo ai grafici a bolle"
type: docs
url: /it/net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

Ottiene o imposta il fattore di scala per le bolle nel gruppo di grafico specificato. Può essere un valore intero da 0 (zero) a 300, corrispondente a una percentuale della dimensione predefinita. Si applica solo ai grafici a bolle.

```csharp
public int BubbleScale { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico a bolle
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["C1"].PutValue("Size");
            
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(5);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["C3"].PutValue(10);
            
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C4"].PutValue(15);

            // Aggiungi un grafico a bolle
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries[seriesIndex].XValues = "A2:A4";
            chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
            
            // Imposta la scala delle bolle per dimostrare la proprietà
            chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
            
            // Personalizza l'aspetto del grafico
            chart.Title.Text = "Bubble Chart with Scaled Bubbles";
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // Salva la cartella di lavoro
            workbook.Save("BubbleScaleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


