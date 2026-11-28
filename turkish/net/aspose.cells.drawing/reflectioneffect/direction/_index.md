---
title: "ReflectionEffect.Direction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReflectionEffect özelliği. Şekle göre alfa gradyan eğiminin yönünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffect/direction/
---
## ReflectionEffect.Direction property

Alfa gradyan rampa yönünü şekle göre alır ve ayarlar.

```csharp
public double Direction { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyDirectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yansıma etkisi uygulamak için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Şeklin yansıma etkisini alın
            ReflectionEffect reflection = shape.Reflection;
            
            // Mevcut Direction değerini göster
            Console.WriteLine("Current Direction value: " + reflection.Direction);
            
            // Yeni Direction değerini ayarlayın (90 derece)
            reflection.Direction = 90;
            Console.WriteLine("New Direction value: " + reflection.Direction);
            
            // Daha iyi görünürlük için diğer yansıma özelliklerini yapılandırın
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            
            // Yansıma etkisini görmek için çalışma kitabını kaydedin
            workbook.Save("ReflectionEffectDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


