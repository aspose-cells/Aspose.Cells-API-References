---
title: "Marker.MarkerStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Marker. Rappresenta lo stile del marcatore. Si applica a un grafico a linee, a dispersione o radar"
type: docs
url: /it/net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

Rappresenta lo stile del marcatore. Si applica a un grafico a linee, un grafico a dispersione o un grafico radar.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["B4"].PutValue(6);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Imposta lo stile del marcatore per la prima serie
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Marker.ForegroundColor = System.Drawing.Color.Blue;
            chart.NSeries[0].Marker.BackgroundColor = System.Drawing.Color.White;
            chart.NSeries[0].Marker.MarkerSize = 10;

            // Salva la cartella di lavoro
            workbook.Save("MarkerStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


