---
title: "ChartFrame.Y"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt die y-Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/chartframe/y/
---
## ChartFrame.Y property

Gibt die y-Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest.

```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```

### Hinweise

Wie konvertiert man Einheiten von 1/4000 in Pixel? Y in Pixel = Y * Chart.ChartObject.Height / 4000d;

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft ChartFrame.YRatioToChart. Y = YRatioToChart * 4000. Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyYDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Diagramm hinzufügen
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Greifen Sie auf den Diagrammtitel zu und setzen Sie die Y-Position
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrate Y property usage

            // Speichere die Arbeitsmappe
            workbook.Save("ChartFramePropertyYDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


