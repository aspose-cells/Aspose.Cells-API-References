---
title: "Klasse SeriesLayoutProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.SeriesLayoutProperties Klasse. Stellt die Eigenschaften des Serienlayouts dar"
type: docs
url: /de/net/aspose.cells.charts/serieslayoutproperties/
---
## SeriesLayoutProperties class

Stellt die Eigenschaften des Serienlayouts dar.

```csharp
public class SeriesLayoutProperties
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SeriesLayoutProperties](serieslayoutproperties/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsIntervalLeftClosed](../../aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/) { get; set; } | Gibt an, ob das Intervall auf der linken Seite geschlossen ist. |
| [MapChartProjectionType](../../aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/) { get; set; } | Liest und setzt den Projektionstyp der Karte. |
| [MapChartRegionType](../../aspose.cells.charts/serieslayoutproperties/mapchartregiontype/) { get; set; } | Liest und setzt den Regionstyp der Karte. |
| [MapLabelLayout](../../aspose.cells.charts/serieslayoutproperties/maplabellayout/) { get; set; } | Liest und setzt das Layout der Kartenbeschriftungen. |
| [QuartileCalculation](../../aspose.cells.charts/serieslayoutproperties/quartilecalculation/) { get; set; } | Stellt die statistischen Eigenschaften für die Serie dar. |
| [ShowConnectorLines](../../aspose.cells.charts/serieslayoutproperties/showconnectorlines/) { get; set; } | Gibt an, ob Verbindungslinien zwischen Datenpunkten angezeigt werden. |
| [ShowInnerPoints](../../aspose.cells.charts/serieslayoutproperties/showinnerpoints/) { get; set; } | Gibt an, ob Nicht-Ausreißer-Datenpunkte angezeigt werden sollen. |
| [ShowMeanLine](../../aspose.cells.charts/serieslayoutproperties/showmeanline/) { get; set; } | Gibt an, ob die Linie angezeigt werden soll, die alle Mittelwertpunkte verbindet. |
| [ShowMeanMarker](../../aspose.cells.charts/serieslayoutproperties/showmeanmarker/) { get; set; } | Gibt an, ob Marker, die den Mittelwert kennzeichnen, angezeigt werden. |
| [ShowOutlierPoints](../../aspose.cells.charts/serieslayoutproperties/showoutlierpoints/) { get; set; } | Gibt an, ob Ausreißer-Datenpunkte angezeigt werden. |
| [Subtotals](../../aspose.cells.charts/serieslayoutproperties/subtotals/) { get; set; } | Stellt den Index eines Zwischensummen-Datenpunkts dar. |

### Hinweise

Nur anwendbar auf BoxWhisker-, Funnel-, ParetoLine-, Sunburst-, Treemap-, Waterfall- und Histogramm-Diagramme.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
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

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Serie zum Diagramm hinzufügen
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];

            // Setze die Werte der Serie
            series.Values = "=B1:B4";

            // Greife auf das SeriesLayoutProperties-Objekt zu
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;

            // Setze Eigenschaften von SeriesLayoutProperties
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

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesLayoutPropertiesExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


