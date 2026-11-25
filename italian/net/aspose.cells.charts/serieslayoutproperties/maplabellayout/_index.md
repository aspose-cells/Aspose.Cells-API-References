---
title: "SeriesLayoutProperties.MapLabelLayout"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesLayoutProperties. Ottiene e imposta il layout delle etichette della mappa"
type: docs
url: /it/net/aspose.cells.charts/serieslayoutproperties/maplabellayout/
---
## SeriesLayoutProperties.MapLabelLayout property

Ottiene e imposta il layout delle etichette della mappa.

```csharp
public MapChartLabelLayout MapLabelLayout { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyMapLabelLayoutDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico della mappa
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("United States");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["A4"].PutValue("Mexico");
            worksheet.Cells["B4"].PutValue(60);

            // Aggiungi un grafico della mappa
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            Series series = chart.NSeries[0];
            series.XValues = "A2:A4";

            // Configura le proprietà di layout della mappa
            series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
            series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            series.LayoutProperties.MapChartRegionType = MapChartRegionType.DataOnly;

            // Salva la cartella di lavoro
            workbook.Save("MapLabelLayoutDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MapChartLabelLayout](../../mapchartlabellayout/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


