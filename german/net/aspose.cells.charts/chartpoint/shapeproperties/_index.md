---
title: "ChartPoint.ShapeProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt das ShapePropertyCollection‑Objekt zurück, das die visuellen Formeigenschaften des ChartPoint enthält."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/shapeproperties/
---
## ChartPoint.ShapeProperties property

Gibt das [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/)‑Objekt zurück, das die visuellen Formeigenschaften des ChartPoint enthält.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ChartPointPropertyShapePropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(100);
            worksheet.Cells["A4"].PutValue(150);

            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "A1:A4";

            // Greife über die Seriensammlung auf den ChartPoint zu.
            ChartPoint chartPoint = chart.NSeries[0].Points[0];
            chartPoint.Shadow = true;

            ShapePropertyCollection shapeProps = chartPoint.ShapeProperties;
            Console.WriteLine("Initial SoftEdgeRadius: " + shapeProps.SoftEdgeRadius);

            shapeProps.SoftEdgeRadius = 8;

            if (shapeProps.HasShadowEffect())
            {
                // Verwende System.Drawing.Color anstelle von PresetColorType.
                shapeProps.ShadowEffect.Color.Color = Color.Red;
                shapeProps.ShadowEffect.Blur = 20;
                shapeProps.ShadowEffect.Distance = 15;
            }

            workbook.Save("ChartPointShapePropertiesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


