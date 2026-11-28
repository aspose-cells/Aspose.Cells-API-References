---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar.

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localfontStyleName | String | Başlık/Altbilgi için yerel yazı tipi stil adı. |
| standardName | String | Standart (en-US yerel ayarı) fonksiyon adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfası için sayfa ayarı seçenekleri oluşturun
            PageSetup pageSetup = worksheet.PageSetup;

            // Bazı metinle bir başlık ayarlayın
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // Küreselleştirme ayarları örneği oluşturun
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // SetStandardHeaderFooterFontStyleName yöntemini çağırın
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // Küreselleştirme ayarlarını çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // Etki, belge oluşturulduğunda veya yazdırıldığında görülecektir
                // Başlıklardaki/altlıklardaki "Arial" yazı tipi stili "Times New Roman" olarak işlenecek
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


