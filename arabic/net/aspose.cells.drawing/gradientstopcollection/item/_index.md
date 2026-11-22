---
title: "GradientStopCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GradientStopCollection. الحصول على نقطة التدرج حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.drawing/gradientstopcollection/item/
---
## GradientStopCollection indexer

يحصل على نقطة التدرج حسب الفهرس.

```csharp
public GradientStop this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

نقطة التدرج.

### أمثلة

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
            
            // عرض استخدام خاصية Item
            GradientStop stop = shape.Fill.GradientFill.GradientStops[1];
            Console.WriteLine("Gradient stop position: " + stop.Position);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GradientStop](../../gradientstop/)
* class [GradientStopCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


