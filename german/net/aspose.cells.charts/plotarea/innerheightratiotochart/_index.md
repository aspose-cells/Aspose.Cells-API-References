---
title: "PlotArea.InnerHeightRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PlotArea-Eigenschaft. Gibt die Höhe des Plotbereichs in Einheiten des Verhältnisses zum Diagrammbereich zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.charts/plotarea/innerheightratiotochart/
---
## PlotArea.InnerHeightRatioToChart property

Liest die Höhe des Plot‑Bereichs aus oder legt sie fest in Einheiten des Verhältnisses zum Diagrammbereich.

```csharp
public double InnerHeightRatioToChart { get; set; }
```

### Hinweise

Der Begrenzungsrahmen des Plot‑Bereichs umfasst den Plot‑Bereich, die Achsenmarkierungen (Achsenbeschriftungen) und einen kleinen Rand um die Achsenmarkierungen herum. Wenn der Wert nicht von MS Excel erstellt wurde, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.

Die **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** und **HeightRatioToChart** von **PlotArea** stellen die Begrenzungsbox des Plotbereichs dar, die den Plotbereich, die Tick-Markierungen (Tick‑Beschriftungen) und einen kleinen Rand um die Tick-Markierungen umfasst. Wenn Sie die tatsächliche Größe des Plotbereichs erhalten möchten, sollten Sie die Eigenschaften **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** und **InnerHeightRatioToChart** aufrufen.

Für Excel 2007 oder neuer ist der Standardwert Null. Sie sollten den Wert erst nach dem Aufruf von Chart.Calculate() abrufen.

InnerHeight in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Hinweis: Wenn InnerHeightRatioToChart gesetzt wird, wird die Eigenschaft IsInnerMode automatisch auf True gesetzt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Auf den Plotbereich zugreifen
            PlotArea plotArea = chart.PlotArea;

            // Den aktuellen Wert von InnerHeightRatioToChart anzeigen
            Console.WriteLine("Current InnerHeightRatioToChart value: " + plotArea.InnerHeightRatioToChart);

            // Einen neuen Wert für InnerHeightRatioToChart festlegen (0,5 = 50 % der Diagrammbereichshöhe)
            plotArea.InnerHeightRatioToChart = 0.5;

            // Demonstrieren Sie die Wirkung, indem Sie die Arbeitsmappe speichern
            workbook.Save("PlotAreaInnerHeightRatioToChartDemo.xlsx");

            // Neuen Wert anzeigen
            Console.WriteLine("New InnerHeightRatioToChart value: " + plotArea.InnerHeightRatioToChart);
        }
    }
}
```

### Siehe auch

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


