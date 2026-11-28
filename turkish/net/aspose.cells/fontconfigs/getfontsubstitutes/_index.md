---
title: "FontConfigs.GetFontSubstitutes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs yöntemi. Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarını içeren bir dizi döndürür."
type: docs
url: /tr/net/aspose.cells/fontconfigs/getfontsubstitutes/
---
## FontConfigs.GetFontSubstitutes method

Orijinal yazı tipi mevcut değilse kullanılacak yazı tipi ikame adlarını içeren bir dizi döndürür.

```csharp
public static string[] GetFontSubstitutes(string originalFontName)
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

    public class FontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // FontConfigs'i başlat
            FontConfigs fontConfigs = new FontConfigs();

            try
            {
                // Bir yazı tipi adıyla GetFontSubstitutes metodunu çağır
                string originalFontName = "Arial";
                string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);

                // Sonuçları görüntüleyin
                Console.WriteLine($"Substitute fonts for '{originalFontName}':");
                if (substitutes != null && substitutes.Length > 0)
                {
                    foreach (string substitute in substitutes)
                    {
                        Console.WriteLine(substitute);
                    }
                }
                else
                {
                    Console.WriteLine("No substitutes found for the specified font.");
                }

                // İkameleri ayarlamayı ve almayı göster
                string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
                FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);

                // Doğrulamak için ikameleri tekrar al
                substitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("\nAfter setting substitutes:");
                foreach (string substitute in substitutes)
                {
                    Console.WriteLine(substitute);
                }
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

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


