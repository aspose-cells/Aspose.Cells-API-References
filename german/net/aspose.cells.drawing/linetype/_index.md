---
title: "Enum LineType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.LineType enum. Enumeriert den Typ des Picture-Randes oder der Chart-Linie"
type: docs
url: /de/net/aspose.cells.drawing/linetype/
---
## LineType enumeration

Enumeriert den Typ des [`Picture`](../picture/) Randes oder der [`Chart`](../../aspose.cells.charts/chart/) Linie.

```csharp
public enum LineType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DarkGray | `6` | Stellt eine dunkelgraue Linie dar. |
| Dash | `1` | Stellt eine Strichlinie dar. |
| DashDot | `3` | Stellt eine Strich-Punkt-Linie dar |
| DashDotDot | `4` | Stellt eine Strich-Punkt-Punkt-Linie dar. |
| Dot | `2` | Stellt eine gepunktete Linie dar. |
| LightGray | `8` | Stellt eine hellgraue Linie dar. |
| MediumGray | `7` | Stellt eine mittelgraue Linie dar. |
| Solid | `0` | Stellt eine durchgezogene Linie dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LineTypeDemo
    {
        public static void LineTypeExample()
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

            // Greifen Sie auf die primäre Kategorienachse zu
            Axis categoryAxis = chart.CategoryAxis;

            // Setzen Sie den Linientyp für die Achsenlinie
            categoryAxis.AxisLine.Style = LineType.DashDot;

            // Setzen Sie die Farbe der Achsenlinie
            categoryAxis.AxisLine.Color = Color.Blue;

            // Zugriff auf die primäre Werteachse
            Axis valueAxis = chart.ValueAxis;

            // Legen Sie den Linientyp für die Hauptgitternetzlinien fest
            valueAxis.MajorGridLines.Style = LineType.Dot;

            // Legen Sie die Farbe der Hauptgitternetzlinien fest
            valueAxis.MajorGridLines.Color = Color.Red;

            // Speichere die Arbeitsmappe
            workbook.Save("LineTypeExample.xlsx");

            // Ergebnisse ausgeben
            Console.WriteLine("Chart created with custom line types for axis and gridlines.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


