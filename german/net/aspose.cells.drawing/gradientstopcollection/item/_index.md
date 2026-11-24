---
title: "GradientStopCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GradientStopCollection‑Eigenschaft. Gibt den Gradient‑Stopp anhand des Index zurück"
type: docs
url: /de/net/aspose.cells.drawing/gradientstopcollection/item/
---
## GradientStopCollection indexer

Ruft den Gradient-Stop anhand des Index ab.

```csharp
public GradientStop this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Der Gradient‑Stopp.

### Beispiele

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
            
            // Demonstriere die Verwendung der Item-Eigenschaft
            GradientStop stop = shape.Fill.GradientFill.GradientStops[1];
            Console.WriteLine("Gradient stop position: " + stop.Position);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [GradientStop](../../gradientstop/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


