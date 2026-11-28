---
title: "ReflectionEffect.FadeDirection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReflectionEffect özelliği. Yansımayı kaydırmak için yönü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffect/fadedirection/
---
## ReflectionEffect.FadeDirection property

Yansımanın kaydırma yönünü alır ve ayarlar.

```csharp
public double FadeDirection { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyFadeDirectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yansıma etkisi uygulamak için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Şeklin yansıma etkisini alın
            ReflectionEffect reflection = shape.Reflection;

            // Mevcut FadeDirection değerini gösterin
            Console.WriteLine("Current FadeDirection value: " + reflection.FadeDirection);

            // Yeni FadeDirection değerini ayarlayın (90 derece)
            reflection.FadeDirection = 90;
            Console.WriteLine("New FadeDirection value: " + reflection.FadeDirection);

            // Daha iyi görünürlük için diğer yansıma özelliklerini yapılandırın
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            reflection.Distance = 10;

            // Etkiyi görmek için çalışma kitabını kaydet
            workbook.Save("ReflectionEffectFadeDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


