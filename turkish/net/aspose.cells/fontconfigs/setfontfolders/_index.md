---
title: "FontConfigs.SetFontFolders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs yöntemi. Yazı tipleri klasörünü ayarlar"
type: docs
url: /tr/net/aspose.cells/fontconfigs/setfontfolders/
---
## FontConfigs.SetFontFolders method

Yazı tipleri klasörünü ayarlar

```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolders | String[] | TrueType yazı tiplerini içeren klasörler. |
| recursive | Boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel yazı tiplerini kullanacak bir metin ayarlayın
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Yazı tipi klasörlerini hazırlayın (sisteminize ait gerçek yollarla değiştirin)
            string[] fontFolders = new string[] 
            {
                @"C:\Windows\Fonts",
                @"D:\CustomFonts"
            };
            bool recursiveSearch = true;

            try
            {
                // String[] ve Boolean parametrelerle SetFontFolders yöntemini çağırın
                FontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Bu klasörlerden birinde olabilecek bir yazı tipini uygulayın
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Replace with actual font name
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folders: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


