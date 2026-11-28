---
title: "FontConfigs.SetFontFolder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs yöntemi. Yazı tipleri klasörünü ayarlar"
type: docs
url: /tr/net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Yazı tipleri klasörünü ayarlar

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolder | String | TrueType yazı tiplerini içeren klasör. |
| recursive | Boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı başlat
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine biraz metin ekleyin
            worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
            
            // Özel yazı tipi klasörünü ayarlayın ve alt klasörlerin dahil edilip edilmeyeceğini belirtin
            FontConfigs.SetFontFolder("Fonts", true);
            
            // Özel klasörden yazı tiplerini kullanabilecek bir yazı tipi stilini uygulayın
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Çalışma kitabını PDF olarak kaydedin
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Ayrıca Bakınız

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


