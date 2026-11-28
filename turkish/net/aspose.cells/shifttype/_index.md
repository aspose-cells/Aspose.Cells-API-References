---
title: "Enum ShiftType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ShiftType enum. Hücre aralığını silerken kaydırma seçeneklerini temsil eder."
type: docs
url: /tr/net/aspose.cells/shifttype/
---
## ShiftType enumeration

Bir hücre aralığını silerken kaydırma seçeneklerini temsil eder.

```csharp
public enum ShiftType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Down | `0` | Hücreleri aşağı kaydır. |
| Left | `1` | Hücreleri sola kaydır. |
| None | `2` | Hücreleri kaydırma. |
| Right | `3` | Hücreleri sağa kaydır. |
| Up | `4` | Hücreleri yukarı kaydır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ShiftTypeDemo
    {
        public static void ShiftTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // 1. indekste yeni bir satır ekle, mevcut satırları aşağı kaydır.
            worksheet.Cells.InsertRows(1, 1, true);

            // Yeni eklenen satıra bir değer ata.
            worksheet.Cells["A1"].PutValue("New Item");

            // Bir hücre aralığını sil ve hücreleri yukarı kaydır
            worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);

            // Kalan değerleri ilk sütunda çıktı olarak ver
            for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
            {
                Console.WriteLine(worksheet.Cells[row, 0].StringValue);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ShiftTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


