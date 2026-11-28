---
title: "FontConfigs.SetFontSources"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs yöntemi. Yazı tipi kaynaklarını ayarlar"
type: docs
url: /tr/net/aspose.cells/fontconfigs/setfontsources/
---
## FontConfigs.SetFontSources method

Yazı tipi kaynaklarını ayarlar.

```csharp
public static void SetFontSources(FontSourceBase[] sources)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynaklar | FontSourceBase[] | TrueType yazı tiplerini içeren kaynakların bir dizisi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Demonstrasyon için geçici bir yazı tipi dosyası oluşturun
            string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
            try
            {
                File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo

                // Yazı tipi kaynakları oluşturun
                FontSourceBase[] fontSources = new FontSourceBase[]
                {
                    new FolderFontSource(Path.GetTempPath(), true),
                    new FileFontSource(tempFontFile)
                };

                try
                {
                    // SetFontSources yöntemini çağırın
                    FontConfigs.SetFontSources(fontSources);

                    // Yazı tipi kaynaklarının ayarlandığını doğrulayın
                    FontSourceBase[] currentSources = FontConfigs.GetFontSources();
                    Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");

                    // Bir yazı tipinin mevcut olup olmadığını kontrol ederek etkiyi gösterin
                    bool isAvailable = FontConfigs.IsFontAvailable("Arial");
                    Console.WriteLine($"Is Arial available: {isAvailable}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
                }
            }
            finally
            {
                // Temizle
                if (File.Exists(tempFontFile))
                {
                    File.Delete(tempFontFile);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


