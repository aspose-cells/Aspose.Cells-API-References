---
title: "PlotArea.XRatioToChart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PlotArea-Eigenschaft. Gibt die x‑koordinate der oberen linken Ecke des Plot‑Bereichs‑Bounding‑Box als Verhältnis zum Diagrammbereich zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.charts/plotarea/xratiotochart/
---
## PlotArea.XRatioToChart property

Liest oder legt die X‑Koordinate der oberen linken Ecke des Begrenzungsrahmens des Plot‑Bereichs als Verhältnis zum Diagrammbereich fest.

```csharp
public override double XRatioToChart { get; set; }
```

### Hinweise

Der Begrenzungsrahmen des Plot‑Bereichs umfasst den Plot‑Bereich, die Achsenmarkierungen (Achsenbeschriftungen) und einen kleinen Rand um die Achsenmarkierungen herum. Wenn der Wert nicht von MS Excel erstellt wurde, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.

Die **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** und **HeightRatioToChart** von **PlotArea** stellen die Begrenzungsbox des Plotbereichs dar, die den Plotbereich, die Tick-Markierungen (Tick‑Beschriftungen) und einen kleinen Rand um die Tick-Markierungen umfasst. Wenn Sie die tatsächliche Größe des Plotbereichs erhalten möchten, sollten Sie die Eigenschaften **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** und **InnerHeightRatioToChart** aufrufen.

Für Excel 2007 oder neuer ist der Standardwert Null. Sie sollten den Wert erst nach dem Aufruf von Chart.Calculate() abrufen.

XPixel = XRatioToChart * chart.ChartObject.Width. Hinweis: Wenn XRatioToChart festgelegt wird, wird die IsInnerMode‑Eigenschaft automatisch auf false gesetzt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyXRatioToChartDemo
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
            chart.SetChartDataRange("A1:B4", true);

            // Den Plotbereich des Diagramms abrufen
            PlotArea plotArea = chart.PlotArea;

            // Zeigen Sie den aktuellen XRatioToChart-Wert an
            Console.WriteLine("Current XRatioToChart value: " + plotArea.XRatioToChart);

            // Ändern Sie den XRatioToChart‑Wert, um den Plot‑Bereich horizontal zu verschieben
            plotArea.XRatioToChart = 0.2; // 20% from the left of the chart area

            // Zeigen Sie den neuen XRatioToChart-Wert an
            Console.WriteLine("New XRatioToChart value: " + plotArea.XRatioToChart);

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("PlotAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


