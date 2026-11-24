---
title: "PlotArea.InnerXRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PlotArea-Eigenschaft. Gibt die x‑koordinate der oberen linken Ecke des Plotbereichs in Einheiten des Verhältnisses zum Diagrammbereich zurück."
type: docs
url: /de/net/aspose.cells.charts/plotarea/innerxratiotochart/
---
## PlotArea.InnerXRatioToChart property

Liest oder legt die X‑Koordinate der oberen Ecke des Plot‑Bereichs in Einheiten des Verhältnisses zum Diagrammbereich fest.

```csharp
public double InnerXRatioToChart { get; set; }
```

### Hinweise

Der Begrenzungsrahmen des Plot‑Bereichs umfasst den Plot‑Bereich, die Achsenmarkierungen (Achsenbeschriftungen) und einen kleinen Rand um die Achsenmarkierungen herum. Wenn der Wert nicht von MS Excel erstellt wurde, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.

Die **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** und **HeightRatioToChart** von **PlotArea** stellen die Begrenzungsbox des Plotbereichs dar, die den Plotbereich, die Tick-Markierungen (Tick‑Beschriftungen) und einen kleinen Rand um die Tick-Markierungen umfasst. Wenn Sie die tatsächliche Größe des Plotbereichs erhalten möchten, sollten Sie die Eigenschaften **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** und **InnerHeightRatioToChart** aufrufen.

Für Excel 2007 oder neuer ist der Standardwert Null. Sie sollten den Wert erst nach dem Aufruf von Chart.Calculate() abrufen.

InnerX in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Hinweis: Wenn InnerXRatioToChart gesetzt wird, wird die Eigenschaft IsInnerMode automatisch auf True gesetzt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerXRatioToChartDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Den Plotbereich des Diagramms abrufen
            PlotArea plotArea = chart.PlotArea;

            // Den aktuellen Wert von InnerXRatioToChart anzeigen
            Console.WriteLine("Current InnerXRatioToChart value: " + plotArea.InnerXRatioToChart);

            // Einen neuen Wert für InnerXRatioToChart festlegen (Plotbereich nach rechts verschieben)
            plotArea.InnerXRatioToChart = 0.2;

            // Den neuen Wert anzeigen
            Console.WriteLine("New InnerXRatioToChart value: " + plotArea.InnerXRatioToChart);

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("PlotAreaPropertyInnerXRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


