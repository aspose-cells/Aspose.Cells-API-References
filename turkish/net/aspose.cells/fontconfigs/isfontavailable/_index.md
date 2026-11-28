---
title: "FontConfigs.IsFontAvailable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs yöntemi. Yazı tipinin mevcut olup olmadığını belirt"
type: docs
url: /tr/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

Yazı tipinin mevcut olup olmadığını belirtin.

```csharp
public static bool IsFontAvailable(string fontName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontName | String | yazı tipi adı |

### Dönüş Değeri

Yazı tipi mevcutsa true, aksi takdirde false.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Mevcudiyetini kontrol etmek için yazı tipi adlarını test et
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // Yazı tipi adıyla IsFontAvailable yöntemini çağır
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // Sonucu göster
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // Sonucu çalışma sayfasına yaz
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


