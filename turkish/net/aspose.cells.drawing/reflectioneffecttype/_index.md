---
title: "Enum ReflectionEffectType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ReflectionEffectType enum. Yansımanın etki tipini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

Yansıma efekt tipini temsil eder.

```csharp
public enum ReflectionEffectType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Yansıma etkisi yok. |
| Custom | `1` | Özel yansıma etkisi. |
| TightReflectionTouching | `2` | Sık yansıma, temaslı. |
| HalfReflectionTouching | `3` | Yarı yansıma, temaslı. |
| FullReflectionTouching | `4` | Tam yansıma, temaslı. |
| TightReflection4PtOffset | `5` | Sık yansıma, 4 pt kaydırma. |
| HalfReflection4PtOffset | `6` | Yarı yansıma, 4 pt kaydırma. |
| FullReflection4PtOffset | `7` | Tam yansıma, 4 pt kaydırma. |
| TightReflection8PtOffset | `8` | Sık yansıma, 8 pt kaydırma. |
| HalfReflection8PtOffset | `9` | Yarı yansıma, 8 pt kaydırma. |
| FullReflection8PtOffset | `10` | Tam yansıma, 8 pt kaydırma. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir dikdörtgen şekli ekle
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Yansıma etkisini al
            ReflectionEffect reflection = rectangle.Reflection;
            
            // Yansıma özelliklerini ayarla
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Çalışma kitabını kaydedin
            workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
            
            Console.WriteLine("Reflection effect demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


