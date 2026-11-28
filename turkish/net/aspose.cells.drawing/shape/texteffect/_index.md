---
title: "Shape.TextEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Belirtilen şekil için metin etkisi biçimlendirme özelliklerini içeren bir TextEffectFormat nesnesi döndürür. WordArt'ı temsil eden Shape nesnelerine uygulanır."
type: docs
url: /tr/net/aspose.cells.drawing/shape/texteffect/
---
## Shape.TextEffect property

Belirtilen şekil için metin etkisi biçimlendirme özelliklerini içeren bir TextEffectFormat nesnesi döndürür. WordArt'ı temsil eden Shape nesnelerine uygulanır.

```csharp
public TextEffectFormat TextEffect { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextEffectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir WordArt şekli ekleyin
            Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);

            // WordArt olup olmadığını kontrol edin ve TextEffect özelliklerine erişin
            if (shape.IsWordArt)
            {
                TextEffectFormat textEffectFormat = shape.TextEffect;
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = true;
                textEffectFormat.FontName = "Arial";
                textEffectFormat.FontSize = 14;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


