---
title: "Klasse TickLabelItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.TickLabelItem Klasse. Stellt ein Tick‑Label im Diagramm dar"
type: docs
url: /de/net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

Stellt ein Tick-Label im Diagramm dar.

```csharp
public class TickLabelItem
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Höhe des Ticklabel‑Elements als Verhältnis zur Diagrammhöhe. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Breite des Ticklabel‑Elements als Verhältnis zur Diagrammbreite. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | X-Koordinaten des Ticklabel-Elements als Verhältnis zur Diagrammbreite. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Y-Koordinaten des Ticklabel-Elements als Verhältnis zur Diagrammhöhe. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartsClassTickLabelItemDemo
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

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen
            chart.Calculate();

            // Zugriff auf die Tick-Labels der Kategorienachse
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Formen hinzufügen, um jede Tick-Label-Position zu markieren
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Rechteck um das Tick-Label hinzufügen
                Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                rectangle.Fill.SolidFill.Transparency = 1;
                rectangle.Line.SolidFill.Color = Color.Blue;

                // Kreis neben dem Tick-Label hinzufügen
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + item.Height,
                    item.Y + item.Height);
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


