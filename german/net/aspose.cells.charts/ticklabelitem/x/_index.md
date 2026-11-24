---
title: "TickLabelItem.X"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabelItem property. X-Koordinaten des Ticklabel-Elements als Verhältnis zur Diagrammbreite"
type: docs
url: /de/net/aspose.cells.charts/ticklabelitem/x/
---
## TickLabelItem.X property

X-Koordinaten des Ticklabel-Elements als Verhältnis zur Diagrammbreite.

```csharp
public double X { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyXDemo
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

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen
            chart.Calculate();

            // Zugriff auf Tick-Label-Elemente
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] items = axis.TickLabels.TickLabelItems;

            // Füge Formen an jeder Tick-Label-Position mithilfe der X-Eigenschaft hinzu
            for (int i = 0; i < items.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = items[i];
                
                // Füge ein Rechteck an der Tick-Label-Position hinzu
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X, 
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Color = Color.LightBlue;
                shape.Line.SolidFill.Color = Color.Blue;

                // Füge einen Kreis neben dem Tick-Label mithilfe der X-Eigenschaft hinzu
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + 0.05, // Small offset
                    item.Y + item.Height);
                
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelItemPropertyXDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


