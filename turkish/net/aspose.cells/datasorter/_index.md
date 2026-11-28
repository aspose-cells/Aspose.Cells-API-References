---
title: "DataSorter sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataSorter sınıfı. DataSorter için özet açıklama"
type: docs
url: /tr/net/aspose.cells/datasorter/
---
## DataSorter class

DataSorter için özet açıklama.

```csharp
public class DataSorter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | Dize karşılaştırılırken büyük/küçük harfe duyarlı olup olmadığını alır ve ayarlar. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | Aralığın başlık içerip içermediğini temsil eder. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | İlk sıralanan sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | İkinci sıralanan sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | Üçüncü sıralanan sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | Veri sıralayıcısının anahtar listesini alır. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | İlk anahtarın sıralama düzenini temsil eder. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | İkinci anahtarın sıralama düzenini temsil eder. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | Üçüncü anahtarın sıralama düzenini temsil eder. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | Sıralamanın sayı gibi görünen şeyleri içerip içermediğini gösterir. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | True, sıralama yönünün soldan sağa olduğunu ifade eder. False, sıralama yönünün üstten alta olduğunu ifade eder. Varsayılan değer false'tur. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | Renk sıralama anahtarı ekler. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | Sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama yönünü ekler. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama yönünü ekler. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama yönünü ekler. |
| [Clear](../../aspose.cells/datasorter/clear/)() | Tüm ayarları temizle. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | Aralıktaki verileri sırala. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | Alan verilerini sırala. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | Alan verilerini sıralar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterDemo
    {
        public static void DataSorterExample()
        {
            // Yeni bir Workbook nesnesi oluştur.
            Workbook workbook = new Workbook("DataSorter_original.xlsx");

            // Workbook DataSorter nesnesini al.
            DataSorter sorter = workbook.DataSorter;

            // DataSorter nesnesi için ilk sıralamayı ayarla.
            sorter.Order1 = SortOrder.Descending;
            // İlk anahtarı tanımla.
            sorter.Key1 = 0;

            // DataSorter nesnesi için ikinci sıralamayı ayarla.
            sorter.Order2 = SortOrder.Ascending;
            // İkinci anahtarı tanımla.
            sorter.Key2 = 1;

            // Bir hücre alanı (aralık) oluştur.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 13,
                EndColumn = 1
            };

            // Belirtilen veri aralığındaki (A1:B14) verileri sırala.
            sorter.Sort(workbook.Worksheets[0].Cells, ca);

            // Excel dosyasını kaydet.
            workbook.Save("DataSorterExample.xlsx");
            workbook.Save("DataSorterExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


