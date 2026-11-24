---
title: "TickLabelItem.Y"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabelItem property. Y-Koordinaten des Ticklabel-Elements als Verhältnis zur Diagrammhöhe"
type: docs
url: /de/net/aspose.cells.charts/ticklabelitem/y/
---
## TickLabelItem.Y property

Y-Koordinaten des Ticklabel-Elements als Verhältnis zur Diagrammhöhe.

```csharp
public double Y { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyYDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            
            // Setze Kategorienachsen-Daten mit NSERIES anstelle von CategoryData
            chart.NSeries.CategoryData = "A1:A3";

            // Diagramm berechnen, um sicherzustellen, dass Tick-Labels erzeugt werden
            chart.Calculate();

            // Hole Tick-Label-Elemente von der Kategorienachse
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;

            // Demonstriere die Verwendung der Y-Eigenschaft, indem Formen hinzugefügt werden, die mit Tick-Labels ausgerichtet sind
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Füge an jeder Y-Position eines Tick-Labels ein Rechteck hinzu
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y, // Using the Y property of TickLabelItem
                    item.X + 0.05, // Small width
                    item.Y + 0.02); // Small height
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


