---
title: "ReflectionEffect.Distance"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReflectionEffect özelliği. Gölgenin ne kadar uzakta olacağını nokta birimi cinsinden alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffect/distance/
---
## ReflectionEffect.Distance property

Gölgenin ne kadar uzakta olacağını alır ve ayarlar, birim olarak puan cinsinden.

```csharp
public double Distance { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ReflectionEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yansımayı test etmek için bir şekil ekle - yöntem imzasına uyması için sabit parametreler
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Yansıma özelliklerini ayarla
            ReflectionEffect reflection = shape.Reflection;
            reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
            reflection.Transparency = 0.5;
            reflection.Size = 55.5;
            reflection.Blur = 0.5;
            reflection.Distance = 4; // Demonstrating Distance property

            // Kalıcı olmayı doğrulamak için kaydet ve yeniden yükle
            string outputPath = "ReflectionEffectDemo.xlsx";
            workbook.Save(outputPath);

            // Doğrulamak için yeniden yükle
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ReflectionEffect loadedReflection = loadedShape.Reflection;

            Console.WriteLine("Original Distance: " + reflection.Distance);
            Console.WriteLine("Loaded Distance: " + loadedReflection.Distance);
        }
    }
}
```

### Ayrıca Bakınız

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


