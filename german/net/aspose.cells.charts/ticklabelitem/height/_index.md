---
title: "TickLabelItem.Height"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabelItem-Eigenschaft. Höhe des Ticklabel-Elements als Verhältnis zur Diagrammhöhe"
type: docs
url: /de/net/aspose.cells.charts/ticklabelitem/height/
---
## TickLabelItem.Height property

Höhe des Ticklabel‑Elements als Verhältnis zur Diagrammhöhe.

```csharp
public double Height { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen
            chart.Calculate();

            // Zugriff auf die Tick-Labels der Kategorienachse
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Formen hinzufügen, um die Höhen der Tick-Label-Elemente zu visualisieren
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Rechteck hinzufügen, das die Begrenzungen des Tick-Label-Elements anzeigt
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;

                // Text hinzufügen, der den Höhenwert anzeigt
                Shape textShape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.TextBox,
                    PlacementType.Move,
                    item.X,
                    item.Y - 0.05, // Position above the tick label
                    0.1,
                    0.05);
                
                textShape.Text = $"H: {item.Height:F4}";
                textShape.Fill.SolidFill.Transparency = 1;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelItemHeightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


