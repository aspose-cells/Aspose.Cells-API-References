---
title: "Sınıf FontConfigs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FontConfigs sınıfı. Yazı tipi ayarlarını belirtir"
type: docs
url: /tr/net/aspose.cells/fontconfigs/
---
## FontConfigs class

Yazı tipi ayarlarını belirtir

```csharp
public class FontConfigs
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FontConfigs](fontconfigs/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Varsayılan yazı tipi adını alır veya ayarlar. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Bir yazı tipi mevcut olmadığında ve bu yazı tipinin ikamesi ayarlanmamış olduğunda sistem yazı tipi ikamelerini önce kullanıp kullanmayacağını belirtin. Örneğin Ubuntu'da "Arial" yazı tipi genellikle "Liberation Sans" ile ikame edilir. Varsayılan değer false'tur. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Yazı tipi dosyası verisinin bilgi verilerini al. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Kaynakların listesini içeren dizinin bir kopyasını alır |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarını içeren bir dizi döndürür. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Yazı tipinin mevcut olup olmadığını belirtin. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Yazı tipleri klasörünü ayarlar |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Yazı tipleri klasörünü ayarlar |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Yazı tipi kaynaklarını ayarlar. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Verilen orijinal yazı tipi adı için ikame yazı tipi adları. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontConfigsDemo
    {
        public static void Run()
        {
            // Özel yazı tipi klasörünü ayarla
            string fontFolder = @"C:\MyFonts\";
            FontConfigs.SetFontFolder(fontFolder, true);

            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı yazı tipleriyle örnek metni ayarla
            worksheet.Cells["A1"].PutValue("Text with default font");
            worksheet.Cells["A2"].PutValue("Text with custom font");
            
            // Özel yazı tipi stilini uygula
            Style style = workbook.CreateStyle();
            style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
            worksheet.Cells["A2"].SetStyle(style);

            // Yazı tipi renderını göstermek için HTML olarak kaydet
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                PresentationPreference = true
            };
            
            workbook.Save("output.html", options);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


