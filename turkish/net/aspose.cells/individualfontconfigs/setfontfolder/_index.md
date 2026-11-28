---
title: "IndividualFontConfigs.SetFontFolder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IndividualFontConfigs yöntemi. Yazı tipleri klasörünü ayarlar"
type: docs
url: /tr/net/aspose.cells/individualfontconfigs/setfontfolder/
---
## IndividualFontConfigs.SetFontFolder method

Yazı tipleri klasörünü ayarlar

```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolder | String | TrueType yazı tiplerini içeren klasör. |
| recursive | Boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // IndividualFontConfigs sınıfının bir örneğini oluşturun
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
            
            // Yazı tipi klasör yolunu ve yinelemeli arama yapılacağını belirtin
            string fontFolderPath = @"C:\Windows\Fonts";
            bool recursiveSearch = true;

            try
            {
                // Belirtilen parametrelerle SetFontFolder metodunu çağırın
                fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
                
                Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
                Console.WriteLine($"Recursive search enabled: {recursiveSearch}");

                // Yazı tipi kullanımını göstermek için bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Belirtilen klasörden yazı tiplerini kullanabilecek bir stil ayarlayın
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
                style.Font.Size = 12;
                
                worksheet.Cells["A1"].Value = "Text with font from specified folder";
                worksheet.Cells["A1"].SetStyle(style);
                
                // Çalışma kitabını kaydedin
                workbook.Save("FontConfigDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folder: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


