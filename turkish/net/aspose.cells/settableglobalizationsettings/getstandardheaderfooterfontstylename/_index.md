---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen yerel yazı tipi stiline göre Başlık/Altbilgi için standart İngilizce yazı tipi stil adı (Normal, Kalın, İtalik) alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Verilen yerel font stiline göre Başlık/Altbilgi için standart İngilizce yazı tipi stil adını (Regular, Bold, Italic) alır.

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localfontStyleName | String | Başlık/Altbilgi için yerel yazı tipi stil adı. |

### Dönüş Değeri

Standart İngilizce yazı tipi stil adı (Normal, Kalın, İtalik)

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Standart bir başlık/altbilgi yazı tipi stil adı eşlemesi ayarlayın
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // Ayarları çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Yerel bir yazı tipi stil adıyla GetStandardHeaderFooterFontStyleName yöntemini çağırın
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // Sonucu göster
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // Yerel yazı tipi stil adıyla bir başlık oluşturun
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // Etkisini elektronik tablo içinde gösterin
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


