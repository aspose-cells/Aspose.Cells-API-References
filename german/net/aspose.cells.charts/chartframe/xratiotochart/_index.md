---
title: "ChartFrame.XRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt die x‑Koordinate der oberen linken Ecke im Verhältnis zur Diagrammfläche zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.charts/chartframe/xratiotochart/
---
## ChartFrame.XRatioToChart property

Liest oder legt fest die x‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses zum Diagrammbereich.

```csharp
public virtual double XRatioToChart { get; set; }
```

### Hinweise

Dies ist ein Bruchwert, sein gültiger Bereich liegt zwischen 0‑1. Wie konvertiert man Verhältnis‑Einheiten in Pixel? XPixel = XRatioToChart * Chart.ChartObject.Width;

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXRatioToChartDemo
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

            // Aktuellen XRatioToChart-Wert anzeigen
            Console.WriteLine("Current XRatioToChart value: " + chartTitle.XRatioToChart);

            // Neuen XRatioToChart‑Wert festlegen (0,5 bedeutet 50 % der Diagrammbreite von links)
            chartTitle.XRatioToChart = 0.5;

            // Neue Position anzeigen
            Console.WriteLine("Title position after change - XRatioToChart: " + chartTitle.XRatioToChart);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartFrameXRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


