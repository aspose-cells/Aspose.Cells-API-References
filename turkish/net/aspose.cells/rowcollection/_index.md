---
title: "Sınıf RowCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.RowCollection sınıfı. Çalışma sayfasındaki bireysel satırları temsil eden Row nesnelerini toplar"
type: docs
url: /tr/net/aspose.cells/rowcollection/
---
## RowCollection class

Çalışma sayfasındaki bireysel satırları temsil eden [`Row`](../row/) nesnelerini toplar.

```csharp
public class RowCollection : IEnumerable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Bu koleksiyondaki satır sayısını alır. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Verilen satır indeksiyle bir [`Row`](../row/) nesnesi alır. Verilen satır indeksine ait Row nesnesi daha önce yoksa oluşturulur. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Tüm satırları ve hücreleri temizleyin. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Bu koleksiyon üzerinden satırları yineleyen bir enumerator alır. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Bu koleksiyon üzerinden satırları yineleyen bir enumerator alır. |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Listedeki konuma göre satır nesnesini alır. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Bu koleksiyondaki belirtilen indeks (konum) konumundaki satır öğesini kaldırın. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionDemo
    {
        public static void RowCollectionExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasının referansını elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // Rows koleksiyonunu al
            RowCollection rows = worksheet.Cells.Rows;

            // Koleksiyondaki satır sayısını al
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // İlk satırı al
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // GetEnumerator kullanarak satırları yineleyin
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // İndexe göre bir satır al
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // Tüm satırları ve hücreleri temizle
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // Çalışma kitabını kaydedin
            workbook.Save("RowCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


