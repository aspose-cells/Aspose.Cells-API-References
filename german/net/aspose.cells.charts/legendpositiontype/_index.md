---
title: "Enum LegendPositionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.LegendPositionType enum. Enumeriert die Legendenpositionsarten"
type: docs
url: /de/net/aspose.cells.charts/legendpositiontype/
---
## LegendPositionType enumeration

Enumeriert die Positionstypen der Legende.

```csharp
public enum LegendPositionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Bottom | `0` | Zeigt die Legende am unteren Rand des Diagrammbereichs an. |
| Corner | `1` | Zeigt die Legende in der Ecke des Diagrammbereichs an. |
| Left | `4` | Zeigt die Legende links vom Diagrammbereich an. |
| NotDocked | `7` | Gibt an, dass die Legende nicht angedockt ist. |
| Right | `3` | Zeigt die Legende rechts vom Diagrammbereich an. |
| Top | `2` | Zeigt die Legende oben im Diagrammbereich an. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPositionTypeDemo
    {
        public static void LegendPositionTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Füge ein Säulendiagramm zum Arbeitsblatt hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Greife auf die Legende des Diagramms zu
            Legend legend = chart.Legend;

            // Setzen Sie die Position der Legende links vom Diagramm
            legend.Position = LegendPositionType.Left;

            // Legen Sie zusätzliche Eigenschaften für die Legende fest
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // Speichere die Arbeitsmappe
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


