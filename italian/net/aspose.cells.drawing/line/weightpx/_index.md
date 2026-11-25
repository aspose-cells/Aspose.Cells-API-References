---
title: "Line.WeightPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Line property. Ottiene o imposta lo spessore della linea in unità di pixel"
type: docs
url: /it/net/aspose.cells.drawing/line/weightpx/
---
## Line.WeightPx property

Ottiene o imposta il peso della linea in unità di pixel.

```csharp
public double WeightPx { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPxDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Aggiungi dati di esempio
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(15);
            cells["B2"].PutValue(25);
            cells["B3"].PutValue(35);

            // Aggiungi un grafico a linee
            int chartIndex = workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura le proprietà della linea con WeightPx
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Border.WeightPx = 5.0; // Set line weight in pixels
            series.Border.Color = System.Drawing.Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("LineWeightPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


