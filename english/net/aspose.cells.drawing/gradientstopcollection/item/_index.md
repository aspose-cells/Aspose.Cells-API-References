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
public GradientStop this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The gradient stop.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GradientStopCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;
            shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            Shape shape = shapes[0];

            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.BottomSpotlight, ThemeColorType.Accent5);
            
            // Demonstrate Item property usage
            GradientStop stop = shape.Fill.GradientFill.GradientStops[1];
            Console.WriteLine("Gradient stop position: " + stop.Position);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [GradientStop](../../gradientstop/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


