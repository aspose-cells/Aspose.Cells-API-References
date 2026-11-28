---
title: "IndividualFontConfigs.GetFontSources"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IndividualFontConfigs yöntemi. Kaynakların listesini içeren dizinin bir kopyasını alır"
type: docs
url: /tr/net/aspose.cells/individualfontconfigs/getfontsources/
---
## IndividualFontConfigs.GetFontSources method

Kaynakların listesini içeren dizinin bir kopyasını alır

```csharp
public FontSourceBase[] GetFontSources()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            // Bireysel yazı tipi yapılandırmaları oluştur
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Bazı yazı tipi kaynaklarını ayarlayın (yazı tiplerini içeren klasörler)
            string fontFolder1 = @"C:\Windows\Fonts";
            string fontFolder2 = @"D:\CustomFonts";
            fontConfigs.SetFontFolder(fontFolder1, false);
            fontConfigs.SetFontFolder(fontFolder2, true);

            try
            {
                // Mevcut yazı tipi kaynaklarını alın
                FontSourceBase[] fontSources = fontConfigs.GetFontSources();

                Console.WriteLine("Current font sources:");
                foreach (var source in fontSources)
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                }

                // Etkiyi göstermek için bir çalışma kitabı oluştur
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                // Stiller oluştururken veya yazı tipleriyle çalışırken yazı tipi yapılandırmalarını kullanın
                // (Workbook'ın FontConfigs özelliği yoktur, bu yüzden bu satırı kaldırıyoruz)
                Worksheet worksheet = workbook.Worksheets[0];

                // Klasörlerden birinde olabilecek özel bir yazı tipi kullanın
                Style style = workbook.CreateStyle();
                style.Font.Name = "SomeCustomFont";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with custom font");

                Console.WriteLine("Workbook created with custom font configurations.");
                workbook.Save("MethodGetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSources method: {ex.Message}");
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


