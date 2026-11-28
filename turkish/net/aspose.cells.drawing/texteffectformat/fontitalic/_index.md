---
title: "TextEffectFormat.FontItalic"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextEffectFormat özelliği. Yazı tipinin italik olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/fontitalic/
---
## TextEffectFormat.FontItalic property

Yazı tipinin italik olup olmadığını gösterir.

```csharp
public bool FontItalic { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontItalicDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin efektiyle bir şekil ekle
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Metin efekti formatını al
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // FontItalic'i true olarak ayarla
            textEffectFormat.FontItalic = true;
            Console.WriteLine("FontItalic after setting to true: " + textEffectFormat.FontItalic);

            // FontItalic'i false olarak ayarla
            textEffectFormat.FontItalic = false;
            Console.WriteLine("FontItalic after setting to false: " + textEffectFormat.FontItalic);

            // Çalışma kitabını kaydedin
            workbook.Save("TextEffectFormatFontItalicDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


