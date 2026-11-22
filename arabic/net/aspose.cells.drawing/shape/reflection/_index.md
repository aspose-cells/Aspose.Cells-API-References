---
title: "Shape.Reflection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل كائن ReflectionEffect الذي يحدد تأثير الانعكاس لعنصر المخطط أو الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/reflection/
---
## Shape.Reflection property

تمثل كائن [`ReflectionEffect`](../../reflectioneffect/) الذي يحدد تأثير الانعكاس لعنصر المخطط أو الشكل.

```csharp
public ReflectionEffect Reflection { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyReflectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // تعيين خصائص الانعكاس
            ReflectionEffect reflection = shape.Reflection;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Direction = 90;
            reflection.FadeDirection = 90;
            reflection.Size = 50;
            reflection.Transparency = 0.5;
            reflection.Type = ReflectionEffectType.None;

            // احفظ المصنف
            workbook.Save("ShapeReflectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


