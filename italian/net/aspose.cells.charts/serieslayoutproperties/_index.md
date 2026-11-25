---
title: "Classe SeriesLayoutProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.SeriesLayoutProperties classe. Rappresenta le proprietà del layout della serie"
type: docs
url: /it/net/aspose.cells.charts/serieslayoutproperties/
---
## SeriesLayoutProperties class

Rappresenta le proprietà del layout della serie.

```csharp
public class SeriesLayoutProperties
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SeriesLayoutProperties](serieslayoutproperties/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsIntervalLeftClosed](../../aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/) { get; set; } | Indica se l'intervallo è chiuso sul lato sinistro. |
| [MapChartProjectionType](../../aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/) { get; set; } | Ottiene e imposta il tipo di proiezione della mappa. |
| [MapChartRegionType](../../aspose.cells.charts/serieslayoutproperties/mapchartregiontype/) { get; set; } | Ottiene e imposta il tipo di regione della mappa. |
| [MapLabelLayout](../../aspose.cells.charts/serieslayoutproperties/maplabellayout/) { get; set; } | Ottiene e imposta il layout delle etichette della mappa. |
| [QuartileCalculation](../../aspose.cells.charts/serieslayoutproperties/quartilecalculation/) { get; set; } | Rappresenta le proprietà statistiche per la serie. |
| [ShowConnectorLines](../../aspose.cells.charts/serieslayoutproperties/showconnectorlines/) { get; set; } | Indica se le linee di collegamento sono visualizzate tra i punti dati. |
| [ShowInnerPoints](../../aspose.cells.charts/serieslayoutproperties/showinnerpoints/) { get; set; } | Indica se mostrare i punti dati non outlier. |
| [ShowMeanLine](../../aspose.cells.charts/serieslayoutproperties/showmeanline/) { get; set; } | Indica se mostrare la linea che collega tutti i punti medi. |
| [ShowMeanMarker](../../aspose.cells.charts/serieslayoutproperties/showmeanmarker/) { get; set; } | Indica se i marcatori che indicano la media sono mostrati. |
| [ShowOutlierPoints](../../aspose.cells.charts/serieslayoutproperties/showoutlierpoints/) { get; set; } | Indica se i punti dati anomali sono mostrati. |
| [Subtotals](../../aspose.cells.charts/serieslayoutproperties/subtotals/) { get; set; } | Rappresenta l'indice di un punto dati subtotale. |

### Osservazioni

Applicabile solo ai grafici BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall e Histogram.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesLayoutPropertiesDemo
    {
        public static void SeriesLayoutPropertiesExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie al grafico
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];

            // Imposta i valori della serie
            series.Values = "=B1:B4";

            // Accedi all'oggetto SeriesLayoutProperties
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;

            // Imposta le proprietà di SeriesLayoutProperties
            layoutProperties.ShowConnectorLines = true;
            layoutProperties.ShowMeanLine = true;
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.QuartileCalculation = QuartileCalculationType.Inclusive;
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            layoutProperties.IsIntervalLeftClosed = true;
            layoutProperties.MapChartRegionType = MapChartRegionType.World;
            layoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Salva la cartella di lavoro
            workbook.Save("SeriesLayoutPropertiesExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


