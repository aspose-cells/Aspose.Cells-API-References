---
title: "ReflectionEffect.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReflectionEffect özelliği. Önceden ayarlanmış yansıma efektini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffect/type/
---
## ReflectionEffect.Type property

Önceden ayarlanmış yansıma etkisini alır ve ayarlar.

```csharp
public ReflectionEffectType Type { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Yansıma efektini al
            ReflectionEffect reflection = shape.Reflection;
            
            // Type özelliğini göster
            Console.WriteLine("Initial reflection type: " + reflection.Type);
            
            // Yansıma tipini değiştir
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            Console.WriteLine("Updated reflection type: " + reflection.Type);
            
            // Diğer yansıma özelliklerini ayarla
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


