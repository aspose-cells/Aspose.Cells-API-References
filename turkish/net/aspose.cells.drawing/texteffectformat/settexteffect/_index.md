---
title: "TextEffectFormat.SetTextEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextEffectFormat metodu. Önceden ayarlanmış metin efektini ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/texteffectformat/settexteffect/
---
## TextEffectFormat.SetTextEffect method

Önceden ayarlanmış metin efektini ayarlar.

```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| efekt | MsoPresetTextEffect | Ön ayarlı metin efekti. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // WordArt için bir şekil ekle
            Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);

            // Şeklin TextEffectFormat'ını al
            TextEffectFormat textEffectFormat = wordArt.TextEffect;

            try
            {
                // MsoPresetTextEffect parametresiyle SetTextEffect metodunu çağır
                textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);

                // WordArt için ek özellikler ayarla
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = false;
                textEffectFormat.FontSize = 24;

                Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


