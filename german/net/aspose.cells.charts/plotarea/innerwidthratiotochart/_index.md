---
title: "PlotArea.InnerWidthRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PlotArea-Eigenschaft. Liest oder setzt die Breite des Plotbereichs in Einheiten des Verhältnisses zum Diagrammbereich."
type: docs
url: /de/net/aspose.cells.charts/plotarea/innerwidthratiotochart/
---
## PlotArea.InnerWidthRatioToChart property

Liest die Breite des Plot‑Bereichs aus oder legt sie fest in Einheiten des Verhältnisses zum Diagrammbereich.

```csharp
public double InnerWidthRatioToChart { get; set; }
```

### Hinweise

Der Begrenzungsrahmen des Plot‑Bereichs umfasst den Plot‑Bereich, die Achsenmarkierungen (Achsenbeschriftungen) und einen kleinen Rand um die Achsenmarkierungen herum. Wenn der Wert nicht von MS Excel erstellt wurde, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.

Die **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** und **HeightRatioToChart** von **PlotArea** stellen die Begrenzungsbox des Plotbereichs dar, die den Plotbereich, die Tick-Markierungen (Tick‑Beschriftungen) und einen kleinen Rand um die Tick-Markierungen umfasst. Wenn Sie die tatsächliche Größe des Plotbereichs erhalten möchten, sollten Sie die Eigenschaften **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** und **InnerHeightRatioToChart** aufrufen.

Für Excel 2007 oder neuer ist der Standardwert Null. Sie sollten den Wert erst nach dem Aufruf von Chart.Calculate() abrufen.

InnerWidth in Pixel = InnerXRatioToChart * chart.ChartObject.Width. Hinweis: Wenn InnerWidthRatioToChart festgelegt wird, wird die Eigenschaft IsInnerMode automatisch auf True gesetzt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerWidthRatioToChartDemo
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
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Auf Plotbereich zugreifen
            PlotArea plotArea = chart.PlotArea;
            
            // Aktuellen InnerWidthRatioToChart-Wert anzeigen
            Console.WriteLine("Current InnerWidthRatioToChart value: " + plotArea.InnerWidthRatioToChart);
            
            // Neuen Wert für InnerWidthRatioToChart festlegen (0,5 bedeutet 50 % der Diagrammbreite)
            plotArea.InnerWidthRatioToChart = 0.5;
            
            // Auswirkung der Änderung anzeigen
            Console.WriteLine("Plot area width changed to 50% of chart width");
            
            // Ergebnis speichern
            workbook.Save("PlotAreaPropertyInnerWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


