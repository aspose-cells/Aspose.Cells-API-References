---
title: "Cell.SetCharacters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücrenin zengin metin biçimini ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/setcharacters/
---
## Cell.SetCharacters method

Hücrenin zengin metin biçimini ayarlar.

```csharp
public void SetCharacters(FontSetting[] characters)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| karakterler | FontSetting[] | Tüm Karakter nesneleri. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellMethodSetCharactersWithFontSettingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Hücre değerini ayarlayarak zengin metin biçimlendirmesi uygulayın
            cell.Value = "Hello World!";

            try
            {
                // Metnin farklı bölümleri için yazı tipi ayarları oluşturun
                FontSetting[] fontSettings = new FontSetting[2];

                // İlk 5 karakteri (Hello) kalın kırmızı olarak biçimlendirin
                fontSettings[0] = cell.Characters(0, 5);
                fontSettings[0].Font.IsBold = true;
                fontSettings[0].Font.Color = Color.Red;

                // Kalan karakterleri ( World!) italik mavi olarak biçimlendirin
                fontSettings[1] = cell.Characters(5, 7);
                fontSettings[1].Font.IsItalic = true;
                fontSettings[1].Font.Color = Color.Blue;

                // Biçimlendirilmiş karakter ayarlarını SetCharacters kullanarak uygulayın
                cell.SetCharacters(fontSettings);

                Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


