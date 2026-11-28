---
title: "FontConfigs.GetFontSources"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs yöntemi. Kaynakların listesini içeren dizinin bir kopyasını alır"
type: docs
url: /tr/net/aspose.cells/fontconfigs/getfontsources/
---
## FontConfigs.GetFontSources method

Kaynakların listesini içeren dizinin bir kopyasını alır

```csharp
public static FontSourceBase[] GetFontSources()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            try
            {
                // Mevcut yazı tipi kaynaklarını alın
                FontSourceBase[] fontSources = FontConfigs.GetFontSources();

                // Her bir yazı tipi kaynağı hakkında bilgileri gösterin
                if (fontSources != null)
                {
                    Console.WriteLine("Current font sources:");
                    foreach (var source in fontSources)
                    {
                        Console.WriteLine($"Type: {source.GetType().Name}");
                        if (source is FolderFontSource folderSource)
                        {
                            Console.WriteLine($"Folder path: {folderSource.FolderPath}");
                            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
                        }
                        else if (source is FileFontSource fileSource)
                        {
                            Console.WriteLine($"File path: {fileSource.FilePath}");
                        }
                        else if (source is MemoryFontSource memorySource)
                        {
                            Console.WriteLine($"Font data present: {memorySource.FontData != null}");
                        }
                        Console.WriteLine();
                    }
                }
                else
                {
                    Console.WriteLine("No font sources are currently set.");
                }

                // Etkiyi göstermek için yeni bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Bu kaynakları kullanabilecek bir yazı tipiyle bazı metinler ayarlayın
                worksheet.Cells["A1"].PutValue("Font Sources Demo");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);

                // Çalışma kitabını kaydedin
                workbook.Save("FontConfigsGetFontSourcesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with font sources: {ex.Message}");
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


