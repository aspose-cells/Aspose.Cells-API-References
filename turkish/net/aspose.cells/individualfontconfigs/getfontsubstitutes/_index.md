---
title: "IndividualFontConfigs.GetFontSubstitutes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IndividualFontConfigs yöntemi. Orijinal font mevcut değilse kullanılacak font ikame adlarını içeren bir dizi döndürür"
type: docs
url: /tr/net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

Orijinal font mevcut değilse kullanılacak font ikame adlarını içeren bir dizi döndürür.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Dönüş Değeri

Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarını içeren bir dizi.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Bireysel yazı tipi yapılandırmaları oluştur
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // "Arial" için font ikamelerini ayarla
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // "Arial" için font ikamelerini al
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // Etkiyi göstermek için bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Orijinal yazı tipiyle bir stil ayarlayın
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // Çalışma kitabını kaydedin
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


