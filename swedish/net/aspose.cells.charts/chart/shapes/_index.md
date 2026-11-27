---
title: "Chart.Shapes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Returnerar alla ritade former i detta diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/shapes/
---
## Chart.Shapes property

Returnerar alla ritningsformer i detta diagram.

```csharp
public ShapeCollection Shapes { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Lägg till en form i diagrammet
            Aspose.Cells.Drawing.Shape shape = chart.Shapes.AddShape(MsoDrawingType.TextBox, 1000, 1000, 2000, 1000, 0, 0);
            shape.Text = "Sample Shape";
            
            // Ändra formegenskaper
            shape.LeftInShape = 4000 - shape.WidthInShape;
            shape.TopInShape = 4000 - shape.HeightInShape;
            
            // Spara arbetsboken
            workbook.Save("ChartPropertyShapesDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


