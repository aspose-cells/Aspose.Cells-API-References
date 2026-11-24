---
title: "Aufzählung ChartMarkerType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ChartMarkerType Enum. Stellt den Markerstil in einem Liniendiagramm, Streudiagramm oder Radardiagramm dar."
type: docs
url: /de/net/aspose.cells.charts/chartmarkertype/
---
## ChartMarkerType enumeration

Stellt den Markierungsstil in einem Liniendiagramm, Streudiagramm oder Radar‑Diagramm dar.

```csharp
public enum ChartMarkerType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Automatische Markierungen. |
| Circle | `1` | Runde Markierungen. |
| Dash | `2` | Lange Balkenmarkierungen |
| Diamond | `3` | Rautenförmige Markierungen. |
| Dot | `4` | Kurze Balkenmarkierungen. |
| None | `5` | Keine Markierungen. |
| SquarePlus | `6` | Quadratische Markierungen mit einem Pluszeichen. |
| Square | `7` | Quadratische Markierungen. |
| SquareStar | `8` | Quadratische Markierungen mit einem Sternchen. |
| Triangle | `9` | Dreieckige Markierungen. |
| SquareX | `10` | Quadratische Markierungen mit einem X. |
| Picture | `11` | Bild |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartMarkerTypeDemo
    {
        public static void ChartMarkerTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Füge die Datenreihe dem Diagramm hinzu
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Zugriff auf den Marker der ersten Serie
            Marker marker = chart.NSeries[0].Marker;

            // Markerstil festlegen
            marker.MarkerStyle = ChartMarkerType.Circle;

            // Markergöße festlegen
            marker.MarkerSize = 10;

            // Vordergrund- und Hintergrundfarben des Markers festlegen
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


