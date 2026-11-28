---
title: "GlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Verilen yerel ayara göre Header/Footer için standart İngilizce yazı tipi stili adı Regular Bold Italic'i alır."
type: docs
url: /tr/net/aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/
---
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Verilen yerel font stiline göre Başlık/Altbilgi için standart İngilizce yazı tipi stil adını (Regular, Bold, Italic) alır.

```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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

    public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel küreselleştirme ayarları örneği oluşturun
            var globalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Parametre tipi (String) ile yöntem çağrısını gösterin
                string localStyle = "CustomBold";
                string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
                Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");

                // Küreselleştirme ayarlarını çalışma kitabına uygulayın
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Dönüştürülecek özel yazı tipi stiliyle üstbilgiyi ayarlayın
                // SetHeader yöntemini bölüm parametresiyle kullanın (0 = sol, 1 = orta, 2 = sağ)
                worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");

                // Etkisini göstermek için çalışma kitabını kaydedin
                workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
        }
    }

    // Özel globalizasyon ayarları uygulaması
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
        {
            // Özel yazı tipi stili adlarını standart adlara dönüştürün
            return localfontStyleName switch
            {
                "CustomBold" => "Bold",
                "CustomItalic" => "Italic",
                _ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
            };
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


