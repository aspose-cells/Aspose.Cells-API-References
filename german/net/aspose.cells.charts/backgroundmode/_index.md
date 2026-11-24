---
title: "Enum BackgroundMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.BackgroundMode enum. Stellt den Anzeigemodus des Hintergrunds dar"
type: docs
url: /de/net/aspose.cells.charts/backgroundmode/
---
## BackgroundMode enumeration

Stellt den Anzeigemodus des Hintergrunds dar.

```csharp
public enum BackgroundMode
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Automatisch |
| Opaque | `1` | Undurchsichtig |
| Transparent | `2` | Transparent |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class BackgroundModeDemo
    {
        public static void BackgroundModeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Holen Sie die Referenz des ersten Arbeitsblatts
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einigen Zellen Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Füge NSeries (Diagrammdatenquelle) zum Diagramm hinzu, das vom Feld "A1" bis "B3" reicht.
            chart.NSeries.Add("A1:B3", true);
            
            // Greifen Sie auf den Diagrammbereich zu
            ChartArea chartArea = chart.ChartArea;

            // Legen Sie die Vordergrundfarbe des Diagrammbereichs fest
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Setzen Sie den Hintergrundmodus des Diagrammbereichs fest
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // Setzen Sie den Schatten des Diagrammbereichs fest
            chartArea.Shadow = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("BackgroundModeExample.xlsx");
            workbook.Save("BackgroundModeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


