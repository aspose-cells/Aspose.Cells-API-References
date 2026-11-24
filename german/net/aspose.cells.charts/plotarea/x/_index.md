---
title: "PlotArea.X"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PlotArea-Eigenschaft. Gibt die x‑koordinate der oberen linken Ecke der Plotbereich‑Begrenzungsbox in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.charts/plotarea/x/
---
## PlotArea.X property

Gibt die x‑koordinate der oberen linken Ecke der Plot‑Bereich‑Begrenzungsbox in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest.

```csharp
[Obsolete("Use PlotArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Hinweise

Der Begrenzungsrahmen des Plot‑Bereichs umfasst den Plot‑Bereich, die Achsenmarkierungen (Achsenbeschriftungen) und einen kleinen Rand um die Achsenmarkierungen herum. Wenn der Wert nicht von MS Excel erstellt wurde, rufen Sie bitte die Methode Chart.Calculate() auf, bevor Sie diese Methode aufrufen.

Die **X**, **Y**, **Width** und **Height** von **PlotArea** stellen die Begrenzungsbox des Plotbereichs dar, die den Plotbereich, die Tick-Markierungen (Tick‑Beschriftungen) und einen kleinen Rand um die Tick-Markierungen umfasst. Wenn Sie die tatsächliche Größe des Plotbereichs erhalten möchten, sollten Sie die Eigenschaften **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** und **InnerHeightRatioToChart** aufrufen.

Für Excel 2007 oder neuer ist der Standardwert Null. Sie sollten den Wert erst nach dem Aufruf von Chart.Calculate() abrufen.

Hinweis: Wenn X gesetzt wird, wird die Eigenschaft IsInnerMode automatisch auf false gesetzt.

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft PlotArea.XRatioToChart. X = XRatioToChart * 4000. Diese Eigenschaft wird 12 Monate nach Februar 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyXDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
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

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // PlotArea-Eigenschaften festlegen
            chart.PlotArea.X = 100;  // Demonstrate X property usage
            chart.PlotArea.Y = 200;
            chart.PlotArea.Width = 1000;
            chart.PlotArea.Height = 800;

            // Speichere die Arbeitsmappe
            workbook.Save("PlotAreaPropertyXDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


