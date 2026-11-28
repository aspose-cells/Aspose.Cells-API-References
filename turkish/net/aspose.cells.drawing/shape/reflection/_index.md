---
title: "Shape.Reflection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Grafik öğesi veya şekil için yansıma etkisini belirten bir ReflectionEffect nesnesini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/reflection/
---
## Shape.Reflection property

Grafik öğesi veya şekil için yansıma etkisini belirten bir [`ReflectionEffect`](../../reflectioneffect/) nesnesini temsil eder.

```csharp
public ReflectionEffect Reflection { get; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Yansıma özelliklerini ayarla
            ReflectionEffect reflection = shape.Reflection;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Direction = 90;
            reflection.FadeDirection = 90;
            reflection.Size = 50;
            reflection.Transparency = 0.5;
            reflection.Type = ReflectionEffectType.None;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeReflectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


