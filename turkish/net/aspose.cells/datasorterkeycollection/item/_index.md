---
title: "DataSorterKeyCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorterKeyCollection özelliği. DataSorterKey'i indeksle alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/datasorterkeycollection/item/
---
## DataSorterKeyCollection indexer

İndeksle [`DataSorterKey`](../../datasorterkey/) alır ve ayarlar.

```csharp
public DataSorterKey this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class DataSorterKeyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["B4"].PutValue(78);

            // Bir liste nesnesi (tablo) oluştur
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Sıralama anahtarı ekle (Score sütununu azalan sırada sırala)
            table.AutoFilter.Sorter.AddKey(1, SortOrder.Descending);
            table.AutoFilter.Sorter.Sort();

            // Item özelliğinin kullanımını göster
            DataSorterKey key = table.AutoFilter.Sorter.Keys[0];
            Console.WriteLine("Sort Key Index: {0}, Order: {1}", key.Index, key.Order);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


