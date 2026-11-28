---
title: "IndividualFontConfigs.SetFontSubstitutes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IndividualFontConfigs yöntemi. Belirli bir orijinal yazı tipi adı için yazı tipi ikame adlarını ayarlar"
type: docs
url: /tr/net/aspose.cells/individualfontconfigs/setfontsubstitutes/
---
## IndividualFontConfigs.SetFontSubstitutes method

Belirli bir orijinal font adı için font ikame adlarını ayarlar.

```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| originalFontName | String | Orijinal yazı tipi adı. |
| substituteFontNames | String[] | Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarının listesi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // IndividualFontConfigs sınıfının bir örneğini oluşturun
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Orijinal yazı tipi adı ve ikameleri
            string originalFont = "Arial";
            string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };

            try
            {
                // Belirtilen parametrelerle SetFontSubstitutes metodunu çağırın
                fontConfigs.SetFontSubstitutes(originalFont, substitutes);

                Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
                Console.WriteLine("Substitutes are:");
                foreach (var sub in substitutes)
                {
                    Console.WriteLine($"- {sub}");
                }

                // Etkiyi göstermek için bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Orijinal yazı tipiyle bir stil ayarlayın
                Style style = workbook.CreateStyle();
                style.Font.Name = originalFont;
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].Value = "This text uses " + originalFont;
                worksheet.Cells["A1"].SetStyle(style);

                // Çalışma kitabını kaydedin
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font substitutes: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


