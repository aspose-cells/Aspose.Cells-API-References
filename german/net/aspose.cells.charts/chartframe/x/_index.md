---
title: "ChartFrame.X"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt die x-Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs zurück oder setzt sie"
type: docs
url: /de/net/aspose.cells.charts/chartframe/x/
---
## ChartFrame.X property

Gibt die x-Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs zurück oder setzt sie.

```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```

### Hinweise

Wie konvertiert man Einheiten von 1/4000 in Pixel? X in Pixel = X * Chart.ChartObject.Width / 4000d;

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.XRatioToChart. X = XRatioToChart * 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyXDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Diagramm hinzufügen
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Fügen Sie Serien hinzu und setzen Sie X/Y-Werte
            chart.NSeries.Add("Sheet1!B2:B10", true);
            chart.NSeries[0].XValues = "Sheet1!A2:A10";

            // Trendlinie hinzufügen
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            
            // Datenbeschriftungen konfigurieren
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Blue;
            
            // Demonstrieren Sie die Verwendung der X-Eigenschaft
            trendline.DataLabels.X = -500; // Set X position offset
            trendline.DataLabels.Y = 200;  // Set Y position offset

            // Speichere die Arbeitsmappe
            workbook.Save("ChartFramePropertyXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


