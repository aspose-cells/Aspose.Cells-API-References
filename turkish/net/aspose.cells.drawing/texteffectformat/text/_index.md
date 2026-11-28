---
title: "TextEffectFormat.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextEffectFormat özelliği. WordArt içindeki metin"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/text/
---
## TextEffectFormat.Text property

WordArt içindeki metin.

```csharp
public string Text { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Metin efekti şekli ekle ve metnini ayarla
            Shape shape = sheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 14, false, false, 0, 0, 0, 0, 100, 100);

            // Metin efektinin metin özelliğine eriş ve değiştir
            shape.TextEffect.Text = "Updated Text";

            // Metnin güncellendiğini doğrula
            Console.WriteLine("Text Effect Content: " + shape.TextEffect.Text);
        }
    }
}
```

### Ayrıca Bakınız

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


