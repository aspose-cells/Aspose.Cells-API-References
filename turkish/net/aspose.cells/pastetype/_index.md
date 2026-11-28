---
title: "Enum PasteType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PasteType enum. Yapıştırma özel türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/pastetype/
---
## PasteType enumeration

Özel yapıştırma türünü temsil eder.

```csharp
public enum PasteType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| All | `0` | Aralığın tüm verilerini kopyalar. |
| Default | `1` | MS Excel'in \"All\" davranışı gibi çalışır. |
| AllExceptBorders | `2` | Aralığın tüm verilerini aralık olmadan kopyalar. |
| DefaultExceptBorders | `3` | MS Excel'in \"All except borders\" davranışı gibi çalışır. |
| ColumnWidths | `4` | Sadece aralığın genişliklerini kopyalar. |
| RowHeights | `5` | Sadece aralığın yüksekliklerini kopyalar. |
| Comments | `6` | Sadece aralıktaki yorumları kopyalar. |
| Formats | `7` | Sadece aralıktaki biçimleri kopyalar. |
| Formulas | `8` | Yalnızca aralıktaki formülleri kopyalar. |
| FormulasAndNumberFormats | `9` | Yalnızca aralıktaki formülleri ve sayı biçimlerini kopyalar. |
| Validation | `10` | Yalnızca aralıktaki doğrulamaları kopyalar. |
| Values | `11` | Yalnızca aralıktaki değerleri kopyalar. |
| ValuesAndFormats | `12` | Yalnızca aralıktaki değerleri ve biçimleri kopyalar. |
| ValuesAndNumberFormats | `13` | Yalnızca aralıktaki değerleri ve sayı biçimlerini kopyalar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Kaynak aralığı tanımla
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // Hedef aralığı tanımla
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // PasteOptions oluştur ve PasteType'ı ayarla
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // Kaynak aralığı, belirtilen PasteOptions ile hedef aralığa kopyala
            destinationRange.Copy(sourceRange, pasteOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("PasteTypeExample.xlsx");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


