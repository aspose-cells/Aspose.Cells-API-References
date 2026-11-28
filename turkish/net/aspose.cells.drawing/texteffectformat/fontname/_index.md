---
title: "TextEffectFormat.FontName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextEffectFormat özelliği. WordArt içinde kullanılan yazı tipinin adı"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/fontname/
---
## TextEffectFormat.FontName property

WordArt içinde kullanılan yazı tipinin adı.

```csharp
public string FontName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir WordArt şekli ekle
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // FontName özelliğini ayarla ve al
            shape.TextEffect.FontName = "+mn-ea";
            string fontName = shape.TextEffect.FontName;

            // Sonucu çıktı olarak ver
            Console.WriteLine("Font Name: " + fontName);
        }
    }
}
```

### Ayrıca Bakınız

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


