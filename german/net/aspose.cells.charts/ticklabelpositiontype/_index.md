---
title: "Enum TickLabelPositionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.TickLabelPositionType enum. Stellt den Positionstyp der Tickmark‑Beschriftungen auf der angegebenen Achse dar."
type: docs
url: /de/net/aspose.cells.charts/ticklabelpositiontype/
---
## TickLabelPositionType enumeration

Stellt den Positionstyp der Tick‑Mark‑Beschriftungen auf der angegebenen Achse dar.

```csharp
public enum TickLabelPositionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| High | `0` | Positionstyp ist hoch. |
| Low | `1` | Positionstyp ist niedrig. |
| NextToAxis | `2` | Positionstyp ist neben der Achse. |
| None | `3` | Positionstyp ist keiner. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelPositionTypeDemo
    {
        public static void TickLabelPositionTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Füge NSeries (Diagrammdatenquelle) zum Diagramm hinzu, das vom Feld "A1" bis "B3" reicht.
            chart.NSeries.Add("A1:B3", true);
            
            // Greife auf die Kategorienachse zu
            Axis categoryAxis = chart.CategoryAxis;
            
            // Setze die Tick‑Beschriftungsposition auf Hoch
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelPositionTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


