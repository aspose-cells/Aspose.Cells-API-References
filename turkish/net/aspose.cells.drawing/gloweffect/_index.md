---
title: "Sınıf GlowEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GlowEffect sınıfı. Bu sınıf, nesnenin kenarlarının dışına renkli bulanık bir kontur eklenen bir parıltı etkisini tanımlar"
type: docs
url: /tr/net/aspose.cells.drawing/gloweffect/
---
## GlowEffect class

Bu sınıf, nesnenin kenarlarının dışına renkli bulanık bir kontur eklenen bir parıltı etkisini belirtir.

```csharp
public class GlowEffect
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | Parıltı etkisinin rengini alır. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsolete.**) Parıltının yarıçapını alır ve ayarlar, birim olarak puan cinsinden. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | Parıltının yarıçapını alır ve ayarlar, birim olarak puan cinsinden. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | Parıltı etkisinin şeffaflık derecesini alır ve ayarlar. 0.0 (opak) ile 1.0 (şeffaf) arasında bir aralık. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GlowEffectDemo
    {
        public static void GlowEffectExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir yay şekli ekleyin
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Yay yerleşimini ayarla
            arcShape.Placement = PlacementType.FreeFloating;

            // Dolgu biçimini ayarla
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // Çizgi stilini ayarla
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // Bir GlowEffect örneği oluştur ve özelliklerini ayarla
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // Çalışma kitabını kaydedin
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


