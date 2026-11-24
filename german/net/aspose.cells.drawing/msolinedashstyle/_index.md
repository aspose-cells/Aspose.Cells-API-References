---
title: "Enum MsoLineDashStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoLineDashStyle enum. Stellt den Stil von Strichlinien dar"
type: docs
url: /de/net/aspose.cells.drawing/msolinedashstyle/
---
## MsoLineDashStyle enumeration

Stellt den Stil von gestrichelten Zeichenlinien dar.

```csharp
public enum MsoLineDashStyle
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Dash | `0` | Stellt eine Strichlinie dar. |
| DashDot | `1` | Stellt eine Strich-Punkt-Linie dar. |
| DashDotDot | `2` | Stellt eine Strich-Punkt-Punkt-Linie dar. |
| DashLongDash | `3` | Stellt eine lange Strich‑kurze Strich-Linie dar. |
| DashLongDashDot | `4` | Stellt eine lange Strich‑kurze Strich‑Punkt-Linie dar. |
| RoundDot | `5` | Stellt eine runde Punkt-Linie dar. |
| Solid | `6` | Stellt eine durchgezogene Linie dar. |
| SquareDot | `7` | Stellt eine quadratische Punkt-Linie dar. |
| Custom | `8` | Benutzerdefinierter Strichstil. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineDashStyleDemo
    {
        public static void MsoLineDashStyleExample()
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

            // Lege den Strichstil der Hauptgitternetzlinien fest
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Lege den Strichstil der Hilfsgitternetzlinien fest
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Speichere die Arbeitsmappe
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // Ergebnisse ausgeben
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


