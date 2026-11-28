---
title: "IndividualFontConfigs.SetFontFolders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IndividualFontConfigs yöntemi. Yazı tipi klasörlerini ayarlar"
type: docs
url: /tr/net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

Font klasörlerini ayarlar

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
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

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // IndividualFontConfigs sınıfının bir örneğini oluşturun
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Yazı tipi klasörleri dizisini hazırlayın
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // String[] ve Boolean parametrelerle SetFontFolders yöntemini çağırın
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Özel bir yazı tipi kullanarak etkiyi gösterin
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


