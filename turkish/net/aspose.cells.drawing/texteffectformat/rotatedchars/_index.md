---
title: "TextEffectFormat.RotatedChars"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextEffectFormat özelliği. true ise belirtilen WordArt'taki karakterler, WordArt'ın sınırlayıcı şekline göre 90 derece döndürülür"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

Doğru ise, belirtilen WordArt'taki karakterler WordArt'ın sınırlayıcı şekline göre 90 derece döndürülür.

```csharp
public bool RotatedChars { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyRotatedCharsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin efektiyle bir şekil ekle
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 100, 100, 200, 50);

            // Metin efekti formatını al
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // RotatedChars özelliğini true olarak ayarla
            textEffectFormat.RotatedChars = true;

            // Çalışma kitabını kaydedin
            workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");

            // RotatedChars özelliğini doğrula
            Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
        }
    }
}
```

### Ayrıca Bakınız

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


