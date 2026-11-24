---
title: "PlotArea.InnerHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PlotArea-Eigenschaft. Gibt die Höhe des Plotbereichs in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/plotarea/innerheight/
---
## PlotArea.InnerHeight property

Gibt die Höhe des Plotbereichs in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest.

```csharp
[Obsolete("Use PlotArea.InnerHeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerHeight { get; set; }
```

### Hinweise

Der Begrenzungsrahmen des Plot‑Bereichs umfasst den Plot‑Bereich, die Achsenmarkierungen (Achsenbeschriftungen) und einen kleinen Rand um die Achsenmarkierungen herum. Wenn der Wert nicht von MS Excel erstellt wurde, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.

Die **X**, **Y**, **Width** und **Height** von **PlotArea** stellen die Begrenzungsbox des Plotbereichs dar, die den Plotbereich, die Tick-Markierungen (Tick‑Beschriftungen) und einen kleinen Rand um die Tick-Markierungen umfasst. Wenn Sie die tatsächliche Größe des Plotbereichs erhalten möchten, sollten Sie die Eigenschaften **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** und **InnerHeightRatioToChart** aufrufen.

Für Excel 2007 oder neuer ist der Standardwert Null. Sie sollten den Wert erst nach dem Aufruf von Chart.Calculate() abrufen.

Hinweis: Wenn InnerHeight festgelegt wird, wird die Eigenschaft IsInnerMode automatisch auf True gesetzt.

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die PlotArea.InnerHeightRatioToChart‑Eigenschaft. InnerHeight = InnerHeightRatioToChart * 4000; Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyInnerHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdaten festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Plotbereich konfigurieren
            PlotArea plotArea = chart.PlotArea;
            plotArea.InnerHeight = 1800; // Demonstrate InnerHeight property
            plotArea.InnerWidth = 2800;
            plotArea.IsInnerMode = true;

            workbook.Save("PlotAreaInnerHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


