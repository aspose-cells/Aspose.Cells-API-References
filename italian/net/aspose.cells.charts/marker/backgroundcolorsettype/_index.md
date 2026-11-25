---
title: "Marker.BackgroundColorSetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Marker. Ottiene o imposta il tipo di set del colore di sfondo del marcatore"
type: docs
url: /it/net/aspose.cells.charts/marker/backgroundcolorsettype/
---
## Marker.BackgroundColorSetType property

Ottiene o imposta il tipo di impostazione del colore di sfondo del marcatore.

```csharp
public FormattingType BackgroundColorSetType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorSetTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Series series = chart.NSeries[seriesIndex];

            // Configura le proprietà del marcatore
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;
            series.Marker.BackgroundColor = System.Drawing.Color.Yellow;

            // Salva la cartella di lavoro
            workbook.Save("MarkerBackgroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


