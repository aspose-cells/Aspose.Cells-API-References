---
title: GradientStopCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: GradientStopCollection property. Gets the gradient stop by the index
type: docs
url: /net/aspose.cells.drawing/gradientstopcollection/item/
---
## GradientStopCollection indexer

Gets the gradient stop by the index.

```csharp
public GradientStop this[int index] { get; set; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The gradient stop.

### Examples

```csharp
// Called: Assert.AreEqual(46, shape.Fill.GradientFill.GradientStops[1].Position);
public void GradientStopCollection_Property_Item()
{
    Workbook workbook = new Workbook();
    ShapeCollection shapes = workbook.Worksheets[0].Shapes;
    shapes.AddRectangle(1, 0, 1, 0, 100, 100);
    Shape shape = shapes[0];

    shape.Fill.FillType = FillType.Gradient;
    shape.Fill.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.BottomSpotlight, ThemeColorType.Accent5);
    Assert.AreEqual(46, shape.Fill.GradientFill.GradientStops[1].Position);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [GradientStop](../../gradientstop/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


