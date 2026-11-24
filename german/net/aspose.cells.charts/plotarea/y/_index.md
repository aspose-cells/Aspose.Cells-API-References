---
title: "PlotArea.Y"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PlotArea-Eigenschaft. Gibt die y‑Koordinate der oberen Ecke des Begrenzungsrahmens des Plotbereichs in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.charts/plotarea/y/
---
## PlotArea.Y property

Gibt die y‑Koordinate der oberen Ecke des Plot‑Bereichs‑Begrenzungsrahmens in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest.

```csharp
[Obsolete("Use PlotArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Hinweise

Der Begrenzungsrahmen des Plot‑Bereichs umfasst den Plot‑Bereich, die Achsenmarkierungen (Achsenbeschriftungen) und einen kleinen Rand um die Achsenmarkierungen herum. Wenn der Wert nicht von MS Excel erstellt wurde, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.

Die **X**, **Y**, **Width** und **Height** von **PlotArea** stellen die Begrenzungsbox des Plotbereichs dar, die den Plotbereich, die Tick-Markierungen (Tick‑Beschriftungen) und einen kleinen Rand um die Tick-Markierungen umfasst. Wenn Sie die tatsächliche Größe des Plotbereichs erhalten möchten, sollten Sie die Eigenschaften **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** und **InnerHeightRatioToChart** aufrufen.

Für Excel 2007 oder neuer ist der Standardwert Null. Sie sollten den Wert erst nach dem Aufruf von Chart.Calculate() abrufen.

Hinweis: Wenn Y gesetzt wird, wird die Eigenschaft IsInnerMode automatisch auf false gesetzt.

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft PlotArea.YRatioToChart. Y = YRatioToChart * 4000. Diese Eigenschaft wird 12 Monate nach Februar 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(50);

            // Diagramm erstellen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Diagrammdaten festlegen
            chart.NSeries.Add("B1:B2", false);
            chart.NSeries.CategoryData = "A1:A2";

            // Plotbereich konfigurieren
            chart.PlotArea.Width = 300;
            chart.PlotArea.Height = 200;
            chart.PlotArea.X = 100;
            chart.PlotArea.Y = 150; // Demonstrating Y property usage

            // Speichere die Arbeitsmappe
            workbook.Save("PlotAreaPropertyYDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


