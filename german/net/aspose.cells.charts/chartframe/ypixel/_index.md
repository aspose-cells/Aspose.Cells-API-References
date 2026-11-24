---
title: "ChartFrame.YPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Liest oder schreibt die y‑Koordinate der oberen linken Ecke in Pixel‑Einheiten"
type: docs
url: /de/net/aspose.cells.charts/chartframe/ypixel/
---
## ChartFrame.YPixel property

Liest oder legt fest die y‑Koordinate der oberen linken Ecke in Einheiten von Pixeln.

```csharp
public virtual int YPixel { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYPixelDemo
    {
        public static void Run()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greifen Sie auf den Diagrammtitel zu (der von ChartFrame erbt)
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;

            // Zeige den aktuellen YPixel-Wert
            Console.WriteLine("Current YPixel value: " + chartFrame.YPixel);

            // Ändere die YPixel‑Position des Diagrammtitels
            chartFrame.YPixel = 50;
            Console.WriteLine("New YPixel value: " + chartFrame.YPixel);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartFrameYPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


