---
title: "TextEffectFormat.PresetShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextEffectFormat özelliği. Önceden tanımlı şekil tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

Önceden ayarlanmış şekil tipini alır ve ayarlar.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyPresetShapeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin efektiyle bir şekil ekle
            Shape shape = worksheet.Shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect1,
                "Sample Text",
                "Arial",
                18,
                false,
                false,
                0,
                0,
                100,
                200,
                0,
                0);

            // Metin efekti formatını al
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // PresetShape özelliğini ayarla ve al
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
            Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);

            // Diğer özellikleri değiştir
            textEffectFormat.Text = "Updated Text";
            textEffectFormat.FontBold = true;
            textEffectFormat.FontSize = 24;

            // Çalışma kitabını kaydedin
            workbook.Save("TextEffectFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


