---
title: "ReflectionEffect.RotWithShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReflectionEffect özelliği. Yansımaların şekille birlikte döndürülüp döndürülmeyeceğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffect/rotwithshape/
---
## ReflectionEffect.RotWithShape property

Yansımanın şekille birlikte döndürülüp döndürülmeyeceğini alır ve ayarlar.

```csharp
public bool RotWithShape { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyRotWithShapeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Yansıma efektini oluştur ve uygula
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.FullReflection4PtOffset;
            reflection.Blur = 5;
            reflection.Distance = 10;
            reflection.Transparency = 0.3;

            // Mevcut RotWithShape değerini göster
            Console.WriteLine("Current RotWithShape value: " + reflection.RotWithShape);

            // RotWithShape değerini true olarak ayarla
            reflection.RotWithShape = true;
            Console.WriteLine("RotWithShape set to: " + reflection.RotWithShape);

            // Etkiyi göstermek için şekli döndür
            shape.RotationAngle = 45;

            // Çalışma kitabını kaydedin
            workbook.Save("ReflectionEffectRotWithShapeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


