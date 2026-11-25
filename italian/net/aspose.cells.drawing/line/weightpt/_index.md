---
title: "Line.WeightPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Ottiene o imposta il peso della linea in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/line/weightpt/
---
## Line.WeightPt property

Ottiene o imposta lo spessore della linea in unità di punti.

```csharp
public double WeightPt { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPtDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura le etichette dei dati
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.HasLeaderLines = true;

            // Personalizza le linee leader
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = Aspose.Cells.Drawing.LineType.Dot;
            series.LeaderLines.WeightPt = 0.25; // Demonstrate WeightPt property
            series.LeaderLines.Color = Color.LightCyan;

            // Salva la cartella di lavoro
            workbook.Save("LeaderLinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


