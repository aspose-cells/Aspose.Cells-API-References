---
title: "SeriesLayoutProperties.ShowMeanMarker"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesLayoutProperties. Indica se i marcatori che indicano la media sono mostrati"
type: docs
url: /it/net/aspose.cells.charts/serieslayoutproperties/showmeanmarker/
---
## SeriesLayoutProperties.ShowMeanMarker property

Indica se i marcatori che indicano la media sono mostrati.

```csharp
public bool ShowMeanMarker { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Crea un grafico (usando il tipo di grafico a colonne che supporta i marcatori della media)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            chart.NSeries.Add("A1:A4", true);
            Series series = chart.NSeries[0];

            // Configura le proprietà di layout con ShowMeanMarker
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowMeanLine = true;

            // Salva l'output
            workbook.Save("ColumnChartWithMeanMarker.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


