---
title: "ChartFrame.HeightRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Liest oder schreibt die Höhe des Rahmens in Einheiten des Verhältnisses zum Diagrammbereich"
type: docs
url: /de/net/aspose.cells.charts/chartframe/heightratiotochart/
---
## ChartFrame.HeightRatioToChart property

Ruft die Höhe des Rahmens im Verhältnis zum Diagrammbereich ab oder legt sie fest.

```csharp
public virtual double HeightRatioToChart { get; set; }
```

### Hinweise

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0‑1. Wie konvertiert man Verhältnis‑Einheiten in Pixel? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greifen Sie auf den Diagrammtitel zu (der von ChartFrame erbt)
            chart.Title.Text = "Sample Chart";
            ChartFrame titleFrame = chart.Title;

            // Zeige den aktuellen HeightRatioToChart-Wert
            Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);

            // Setze ein neues HeightRatioToChart-Verhältnis (0,1 = 10 % der Diagrammhöhe)
            titleFrame.HeightRatioToChart = 0.1;

            // Demonstriere die Wirkung durch Vergleich von Vorher/Nachher
            Console.WriteLine("Title height reduced to 10% of chart height");

            // Ergebnis speichern
            workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


