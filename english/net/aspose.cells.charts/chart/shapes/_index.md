---
title: Chart.Shapes
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Returns all drawing shapes in this chart
type: docs
url: /net/aspose.cells.charts/chart/shapes/
---
## Chart.Shapes property

Returns all drawing shapes in this chart.

```csharp
public ShapeCollection Shapes { get; }
```

### Examples

```csharp
// Called: Shape shape = workbook.Worksheets[0].Charts[0].Shapes[0];
public void Chart_Property_Shapes()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "TestMovingShapeInChart.xls");
    Shape shape = workbook.Worksheets[0].Charts[0].Shapes[0];
    shape.LeftInShape = 4000 - shape.WidthInShape;
    shape.TopInShape = 4000 - shape.HeightInShape;
    Assert.AreEqual(4000, shape.LeftInShape + shape.WidthInShape);
    workbook.Save(Constants.destPath + "TestMovingShapeInChart.xls");
}
```

### See Also

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


