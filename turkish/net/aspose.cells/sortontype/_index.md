---
title: "Enum SortOnType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.SortOnType enum. Sıralanmış değer tipi"
type: docs
url: /tr/net/aspose.cells/sortontype/
---
## SortOnType enumeration

Sıralanmış değer türü.

```csharp
public enum SortOnType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Value | `0` | Hücrelerin değerine göre sıralar. |
| CellColor | `1` | Hücrelerin rengine göre sıralar. |
| FontColor | `2` | Hücrelerin yazı tipi rengine göre sıralar. |
| Icon | `3` | Koşullu simgeye göre sıralar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SortOnTypeDemo
    {
        public static void SortOnTypeExample()
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

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(95);
            worksheet.Cells["B4"].PutValue(75);

            // Aralığa otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:B4";

            // Otomatik filtreyi al
            AutoFilter autoFilter = worksheet.AutoFilter;

            // Veri sıralayıcısını al
            DataSorter sorter = autoFilter.Sorter;

            // İlk anahtarı, ikinci sütundaki (Score) değerlere göre sıralamak için ayarla
            sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);

            // Aralıktaki verileri sırala
            sorter.Sort(worksheet.Cells, 1, 0, 3, 1);

            // Çalışma kitabını kaydedin
            workbook.Save("SortOnTypeExample.xlsx");

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Data sorted by Score in descending order.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


