---
title: "Enum LineJoinType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.LineJoinType enum. Stellt die Verbindungsstile einer Linie dar."
type: docs
url: /de/net/aspose.cells.drawing/linejointype/
---
## LineJoinType enumeration

Stellt die Verbindungsstile einer Linie dar.

```csharp
public enum LineJoinType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Round | `0` | Runder Anschluss |
| Bevel | `1` | Fasenverbindung |
| Miter | `2` | Gehrungsverbindung |
| None | `3` | Keine Verbindung |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LineJoinTypeDemo
    {
        public static void LineJoinTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Zugriff auf die primäre Werteachse
            Axis valueAxis = chart.ValueAxis;

            // Zugriff auf das Linienformat der Hauptgitternetzlinien
            Line majorGridLines = valueAxis.MajorGridLines;

            // Den Verbindungstyp der Linie festlegen
            majorGridLines.JoinType = LineJoinType.Round;

            // Den Verbindungstyp ausgeben
            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);

            // Speichere die Arbeitsmappe
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


