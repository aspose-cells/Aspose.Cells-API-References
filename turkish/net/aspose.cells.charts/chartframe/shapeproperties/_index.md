---
title: "ChartFrame.ShapeProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. ShapeProperties nesnesini alır"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/shapeproperties/
---
## ChartFrame.ShapeProperties property

`ShapeProperties` nesnesini alır.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyShapePropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);

            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B2", true);

            PlotArea plotArea = chart.PlotArea;
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            Bevel topBevel = shapeProperties.Format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 8;

            workbook.Save("ChartFramePropertyShapePropertiesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


