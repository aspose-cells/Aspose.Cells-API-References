---
title: "ReflectionEffect.Size"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReflectionEffect özelliği. Yüzde birimi cinsinden alfa gradyan rampası boyunca son alfa değerinin son konumunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffect/size/
---
## ReflectionEffect.Size property

Alfa gradyan rampası boyunca son alfa değerinin bitiş konumunu alır ve ayarlar, yüzde biriminde.

```csharp
public double Size { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir shape ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Yansıma özelliklerini, Size dahil, ayarla
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4;

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // Kaydedilen yansıma özelliklerini doğrula
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Reflection Size: " + loadedReflection.Size);
        }
    }
}
```

### Ayrıca Bakınız

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


