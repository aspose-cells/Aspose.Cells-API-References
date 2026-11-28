---
title: "Class ShadowEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShadowEffect class. Bu sınıf, grafik öğesinin veya şeklinin gölge etkisini belirtir."
type: docs
url: /tr/net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

Bu sınıf grafik öğesinin veya şeklin gölge etkisini belirtir.

```csharp
public class ShadowEffect
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Aydınlatma açısını alır ve ayarlar. Aralık 0 ile 359,9 derece arasındadır. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Gölgenin bulanıklığını alır ve ayarlar. 0 ile 100 puan arasında. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Gölgenin rengini alır ve ayarlar. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Gölgenin mesafesini alır ve ayarlar. 0 ile 200 puan arasında. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Gölgenin önceden ayarlanmış gölge tipini alır ve ayarlar. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Gölgenin boyutunu alır ve ayarlar. Aralık 0 ile 2.0 arasındadır. İç gölgede anlamı yoktur. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Gölgenin şeffaflık derecesini alır ve ayarlar. Aralık 0.0 (opak) ile 1.0 (şeffaf) arasındadır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShadowEffectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir örnek şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Şeklin gölge etkisini al
            ShadowEffect shadow = shape.ShadowEffect;

            // Gölge özelliklerini ayarla
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            Console.WriteLine("Shadow effect demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


