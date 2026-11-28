---
title: "Sınıf TextEffectFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.TextEffectFormat sınıfı. WordArt nesnelerine uygulanan özellik ve yöntemleri içerir"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/
---
## TextEffectFormat class

WordArt nesnelerine uygulanan özellikleri ve yöntemleri içerir.

```csharp
public class TextEffectFormat
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | Yazı tipinin kalın olup olmadığını gösterir. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | Yazı tipinin italik olup olmadığını gösterir. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | WordArt içinde kullanılan yazı tipinin adı. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | WordArt içinde kullanılan yazı tipinin boyutu (puan cinsinden). |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | Önceden ayarlanmış şekil tipini alır ve ayarlar. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | Doğru ise, belirtilen WordArt'taki karakterler WordArt'ın sınırlayıcı şekline göre 90 derece döndürülür. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | WordArt içindeki metin. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | Önceden ayarlanmış metin efektini ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextEffectFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            
            // Metin efekti şekli ekle
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            
            // Metin efektini değiştir
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;
            textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
            
            // Çalışma kitabını kaydedin
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


