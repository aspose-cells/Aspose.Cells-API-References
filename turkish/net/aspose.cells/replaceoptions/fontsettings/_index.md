---
title: "ReplaceOptions.FontSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReplaceOptions özelliği. Değiştirilen metin için zengin biçimlendirilmiş ayarlar"
type: docs
url: /tr/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

Değiştirilen metin için zengin biçimlendirilmiş ayarlar.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyFontSettingsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine örnek metin ayarlayın
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // Yazı tipi ayarlarıyla değiştirme seçenekleri oluştur
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // Değiştirme metni için yazı tipi ayarı oluştur
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // Yazı tipi ayarlarını değiştirme seçeneklerine uygula
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // Değiştirmeyi gerçekleştir
            workbook.Replace("text", "REPLACED", options);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


