---
title: "ReflectionEffect.Blur"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReflectionEffect özelliği. Bulanıklık yarıçapını nokta birimi cinsinden alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffect/blur/
---
## ReflectionEffect.Blur property

Bulanıklık yarıçapını alır ve ayarlar, birim olarak puan cinsinden.

```csharp
public double Blur { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir dikdörtgen şekli ekle
            Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Yansıma efektine eriş
            Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
            
            // Yansıma tipini ve özelliklerini ayarla
            reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
            reflection.Blur = 0.5; // Demonstrate Blur property
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Distance = 0;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ReflectionEffectDemo.xlsx");
            
            // Bulanıklık değerini göster
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
        }
    }
}
```

### Ayrıca Bakınız

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


