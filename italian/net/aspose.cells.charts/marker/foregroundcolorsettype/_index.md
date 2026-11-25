---
title: "Marker.ForegroundColorSetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Marker. Ottiene o imposta il tipo di set del colore di primo piano del marcatore"
type: docs
url: /it/net/aspose.cells.charts/marker/foregroundcolorsettype/
---
## Marker.ForegroundColorSetType property

Ottiene o imposta il tipo di impostazione del colore di primo piano del marcatore.

```csharp
public FormattingType ForegroundColorSetType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyForegroundColorSetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            chart.NSeries.Add("A1:B3", true);
            
            // Configura il marcatore della serie
            Series series = chart.NSeries[0];
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;

            workbook.Save("MarkerForegroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


