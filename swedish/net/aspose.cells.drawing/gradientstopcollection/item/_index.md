---
title: "GradientStopCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientStopCollection‑egenskap. Hämtar gradientstoppet efter index"
type: docs
url: /sv/net/aspose.cells.drawing/gradientstopcollection/item/
---
## GradientStopCollection indexer

Hämtar gradientstoppet efter indexet.

```csharp
public GradientStop this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Gradientstoppet.

### Exempel

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
            
            // Demonstrera användning av Item-egenskapen
            GradientStop stop = shape.Fill.GradientFill.GradientStops[1];
            Console.WriteLine("Gradient stop position: " + stop.Position);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [GradientStop](../../gradientstop/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


