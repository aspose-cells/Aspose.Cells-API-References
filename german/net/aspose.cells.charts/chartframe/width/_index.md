---
title: "ChartFrame.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Liest oder setzt die Breite des Rahmens in Einheiten von 1/4000 des Diagrammbereichs"
type: docs
url: /de/net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Liest oder setzt die Breite des Rahmens in Einheiten von 1/4000 des Diagrammbereichs.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Hinweise

Wie konvertiert man Einheiten von 1/4000 in Pixel? Breite in Pixeln = Breite * Chart.ChartObject.Height / 4000d;

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die ChartFrame.WidthRatioToChart-Eigenschaft. Width = WidthRatioToChart * 4000; Diese Eigenschaft wird 12 Monate nach Februar 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Fügen Sie ein Diagramm hinzu und erhalten Sie dessen ChartFrame
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            ChartFrame chartFrame = chart.ChartArea;

            // Setze und zeige die ursprüngliche Breite an
            chartFrame.Width = 800;
            Console.WriteLine("Original Width: " + chartFrame.Width);

            // Ändere die Breite
            chartFrame.Width = 1000;
            Console.WriteLine("Modified Width: " + chartFrame.Width);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartFrameWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


