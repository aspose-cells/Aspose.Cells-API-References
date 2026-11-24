---
title: "ChartFrame.WidthRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Ermittelt oder legt die Breite des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich fest."
type: docs
url: /de/net/aspose.cells.charts/chartframe/widthratiotochart/
---
## ChartFrame.WidthRatioToChart property

Liest oder legt fest die Breite des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich.

```csharp
public virtual double WidthRatioToChart { get; set; }
```

### Hinweise

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0‑1. Wie konvertiert man Verhältnis‑Einheiten in Pixel? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greifen Sie auf den Diagrammtitel zu, der ein ChartFrame ist
            ChartFrame chartTitle = chart.Title;

            // Zeigen Sie das aktuelle Breitenverhältnis an
            Console.WriteLine("Current WidthRatioToChart value: " + chartTitle.WidthRatioToChart);

            // Setzen Sie ein neues Breitenverhältnis (0,5 = 50 % der Diagrammbreite)
            chartTitle.WidthRatioToChart = 0.5;

            // Zeigen Sie den Effekt, indem Sie die Arbeitsmappe speichern
            workbook.Save("ChartFrameWidthRatioDemo.xlsx");

            Console.WriteLine("WidthRatioToChart property demonstrated successfully.");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


