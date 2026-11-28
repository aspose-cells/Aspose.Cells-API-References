---
title: "Sınıf ReflectionEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ReflectionEffect sınıfı. Bu sınıf bir yansıma etkisi belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

Bu sınıf bir yansıma etkisini belirtir.

```csharp
public class ReflectionEffect
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Bulanıklık yarıçapını alır ve ayarlar, birim olarak puan cinsinden. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Alfa gradyan rampa yönünü şekle göre alır ve ayarlar. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Gölgenin ne kadar uzakta olacağını alır ve ayarlar, birim olarak puan cinsinden. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Yansımanın kaydırma yönünü alır ve ayarlar. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Yansımanın şekille birlikte döndürülüp döndürülmeyeceğini alır ve ayarlar. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Alfa gradyan rampası boyunca son alfa değerinin bitiş konumunu alır ve ayarlar, yüzde biriminde. |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Başlangıç yansıma şeffaflığının derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır ve ayarlar. |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Önceden ayarlanmış yansıma etkisini alır ve ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Yansıma etkisi özelliklerini ayarla
            ReflectionEffect reflection = shape.Reflection;
            reflection.Size = 90;
            reflection.Blur = 30;
            reflection.Transparency = 0.5;
            reflection.Distance = 10;

            // Yansıma özelliklerini göster
            Console.WriteLine("Reflection Size: " + reflection.Size);
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
            Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
            Console.WriteLine("Reflection Distance: " + reflection.Distance);

            // Çalışma kitabını kaydedin
            workbook.Save("ReflectionEffectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


