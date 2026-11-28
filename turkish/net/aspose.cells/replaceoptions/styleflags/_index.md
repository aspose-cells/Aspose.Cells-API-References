---
title: "ReplaceOptions.StyleFlags"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReplaceOptions özelliği. Yazı tipi ayarlarını uygulama bayraklarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

Yazı tipi ayarlarının uygulanma bayraklarını alır ve ayarlar.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyStyleFlagsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücreye örnek metin ekle
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // Değiştirme seçenekleri oluştur
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // Yazı tipi ayarı ve stil bayrağı oluştur
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // Yazı tipini ve stili yapılandır
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // Ayarları seçeneklere uygula
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // Değiştirmeyi gerçekleştir
            workbook.Replace("test", replacementText, options);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


