---
title: "Cell.Replace"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücrenin metnini seçeneklerle değiştir"
type: docs
url: /tr/net/aspose.cells/cell/replace/
---
## Cell.Replace method

Hücrenin metnini seçeneklerle değiştir.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| Yer tutucu | String | Hücre yer tutucu |
| yeniDeğer | String | Değiştirilecek dize değeri |
| seçenekler | ReplaceOptions | Değiştirme seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // Değiştirme seçenekleri oluştur
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // B1 hücresinden yazı tipi ayarlarını al ve değişikliklere uygula
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // Seçenekleri kullanarak "hello"nun tüm varyasyonlarını "Hi" ile değiştir
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


