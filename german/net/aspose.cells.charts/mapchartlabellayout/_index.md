---
title: "Enum MapChartLabelLayout"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.MapChartLabelLayout enum. Stellt das Layout der Karten-Diagramm-Beschriftungen dar"
type: docs
url: /de/net/aspose.cells.charts/mapchartlabellayout/
---
## MapChartLabelLayout enumeration

Stellt das Layout der Beschriftungen des Karten‑Diagramms dar.

```csharp
public enum MapChartLabelLayout
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| BestFitOnly | `0` | Nur die beste Anpassung wird verwendet. |
| ShowAll | `1` | Zeigt alle Beschriftungen an. |
| None | `2` | Es gibt keine Beschriftungen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartLabelLayoutDemo
    {
        public static void MapChartLabelLayoutExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Karten‑Diagramm hinzufügen.
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Füge ein Karten‑Diagramm zum Arbeitsblatt hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich für das Diagramm fest
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greife auf die Layout‑Eigenschaften der Serie zu
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Legen Sie das Beschriftungs‑Layout des Karten‑Diagramms fest.
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;

            // Speichere die Arbeitsmappe
            workbook.Save("MapChartLabelLayoutExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


