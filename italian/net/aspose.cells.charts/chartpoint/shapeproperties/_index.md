---
title: "ChartPoint.ShapeProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene l'oggetto ShapePropertyCollection che contiene le proprietà visive della forma del ChartPoint"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shapeproperties/
---
## ChartPoint.ShapeProperties property

Ottiene l'oggetto [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/) che contiene le proprietà visive della forma del ChartPoint.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Esempi

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

            // Accedi al punto del grafico tramite la raccolta di serie
            ChartPoint chartPoint = chart.NSeries[0].Points[0];
            chartPoint.Shadow = true;

            ShapePropertyCollection shapeProps = chartPoint.ShapeProperties;
            Console.WriteLine("Initial SoftEdgeRadius: " + shapeProps.SoftEdgeRadius);

            shapeProps.SoftEdgeRadius = 8;

            if (shapeProps.HasShadowEffect())
            {
                // Usa System.Drawing.Color al posto di PresetColorType
                shapeProps.ShadowEffect.Color.Color = Color.Red;
                shapeProps.ShadowEffect.Blur = 20;
                shapeProps.ShadowEffect.Distance = 15;
            }

            workbook.Save("ChartPointShapePropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


