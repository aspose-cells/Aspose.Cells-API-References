---
title: "Enum TickMarkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.TickMarkType enum. Stellt den Tick-Mark-Typ für die angegebene Achse dar"
type: docs
url: /de/net/aspose.cells.charts/tickmarktype/
---
## TickMarkType enumeration

Stellt den Tick‑Mark‑Typ für die angegebene Achse dar.

```csharp
public enum TickMarkType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Cross | `0` | Tick-Mark-Typ ist Kreuz. |
| Inside | `1` | Tick-Mark-Typ ist Innen. |
| None | `2` | Tick-Mark-Typ ist Keine. |
| Outside | `3` | Tick-Mark-Typ ist Außen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickMarkTypeDemo
    {
        public static void TickMarkTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
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

            // Zugriff auf die Werteachse des Diagramms
            Axis valueAxis = chart.ValueAxis;

            // Setzen Sie den Haupt Tick-Mark-Typ auf Kreuz
            valueAxis.MajorTickMark = TickMarkType.Cross;

            // Setzen Sie den Neben Tick-Mark-Typ auf Innen
            valueAxis.MinorTickMark = TickMarkType.Inside;

            // Legen Sie den Maximalwert der Werteachse fest
            valueAxis.MaxValue = 200;

            // Legen Sie den Minimalwert der Werteachse fest
            valueAxis.MinValue = 0;

            // Legen Sie die Haupteinheit fest
            valueAxis.MajorUnit = 25;

            // Speichere die Arbeitsmappe
            workbook.Save("TickMarkTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


