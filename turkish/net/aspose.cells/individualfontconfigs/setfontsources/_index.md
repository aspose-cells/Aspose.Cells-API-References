---
title: "IndividualFontConfigs.SetFontSources"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IndividualFontConfigs yöntemi. Yazı tipi kaynaklarını ayarlar"
type: docs
url: /tr/net/aspose.cells/individualfontconfigs/setfontsources/
---
## IndividualFontConfigs.SetFontSources method

Yazı tipi kaynaklarını ayarlar.

```csharp
public void SetFontSources(FontSourceBase[] sources)
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

    public class IndividualFontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Bireysel yazı tipi yapılandırmaları oluştur
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Yazı tipi kaynaklarını hazırla - hem klasör hem de bellek yazı tipi kaynaklarını kullanarak
            FontSourceBase[] fontSources = new FontSourceBase[]
            {
                new FolderFontSource(@"C:\Windows\Fonts", false),
                new MemoryFontSource(File.ReadAllBytes(@"C:\Windows\Fonts\arial.ttf"))
            };

            try
            {
                // Hazırlanan yazı tipi kaynaklarıyla SetFontSources'ı çağır
                fontConfigs.SetFontSources(fontSources);

                Console.WriteLine("Font sources set successfully:");
                foreach (var source in fontConfigs.GetFontSources())
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                    else if (source is MemoryFontSource memorySource)
                    {
                        Console.WriteLine($"- Memory font with data length: {memorySource.FontData.Length} bytes");
                    }
                }

                // Etkiyi göstermek için bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Kaynaklardan mevcut olması gereken bir yazı tipi kullan
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "Text using font from custom sources";
                worksheet.Cells["A2"].Value = "This demonstrates SetFontSources with FontSourceBase[]";

                // Çalışma kitabını kaydedin
                workbook.Save("SetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


