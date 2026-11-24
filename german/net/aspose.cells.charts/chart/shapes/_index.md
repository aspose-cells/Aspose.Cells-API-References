---
title: "Chart.Shapes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt alle Zeichenformen in diesem Diagramm zurück."
type: docs
url: /de/net/aspose.cells.charts/chart/shapes/
---
## Chart.Shapes property

Liefert alle Zeichenformen in diesem Diagramm.

```csharp
public ShapeCollection Shapes { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyShapesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Füge dem Diagramm eine Form hinzu.
            Aspose.Cells.Drawing.Shape shape = chart.Shapes.AddShape(MsoDrawingType.TextBox, 1000, 1000, 2000, 1000, 0, 0);
            shape.Text = "Sample Shape";
            
            // Formeigenschaften ändern.
            shape.LeftInShape = 4000 - shape.WidthInShape;
            shape.TopInShape = 4000 - shape.HeightInShape;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartPropertyShapesDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


