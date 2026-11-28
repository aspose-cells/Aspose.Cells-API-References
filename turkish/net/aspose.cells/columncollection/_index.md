---
title: "Sınıf ColumnCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ColumnCollection sınıfı. Çalışma sayfasındaki bireysel sütun ayarlarını temsil eden Column nesnelerinin koleksiyonu. Column nesnesi yalnızca sütun genişliği, stil vb. gibi tüm sütun için ayarları temsil eder; ilgili sütunda boş olmayan hücre verileri olup olmamasıyla hiçbir ilgisi yoktur. Ve bu koleksiyonun Count özelliği yalnızca bu koleksiyonda örneklenmiş Column nesnelerinin sayısını temsil eder; çalışma sayfasında boş olmayan hücre verileri olup olmamasıyla hiçbir ilgisi yoktur."
type: docs
url: /tr/net/aspose.cells/columncollection/
---
## ColumnCollection class

Collection of the [`Column`](../column/) nesnelerinin, bir çalışma sayfasındaki bireysel sütun (ayar)larını temsil eden koleksiyonu. Column nesnesi yalnızca sütun genişliği, stiller vb. gibi tüm sütun için ayarları temsil eder; ilgili sütunda boş olmayan hücre (veri) olup olmamasıyla hiçbir ilgisi yoktur. Ve bu koleksiyonun "Count" özelliği yalnızca bu koleksiyonda örneklenmiş Column nesnelerinin sayısını temsil eder; çalışma sayfasında boş olmayan hücre (veri) olup olmamasıyla hiçbir ilgisi yoktur.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/columncollection/item/) { get; } | Verilen sütun indeksiyle bir [`Column`](../column/) nesnesi alır. Belirtilen sütun indeksi için Column nesnesi daha önce mevcut değilse oluşturulur. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [GetByIndex](../../aspose.cells/columncollection/getbyindex/)(int) | (**Obsolete.**) İndeks ile sütun nesnesini alır. |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex/)(int) | Listedeki konuma göre [`Column`](../column/) nesnesini alır. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnCollectionDemo
    {
        public static void ColumnCollectionExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasının referansını elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma kitabına yeni Stil ekle
            Style style = workbook.CreateStyle();

            // Arka plan rengini Mavi olarak ayarlama.
            style.ForegroundColor = Color.Blue;

            // Arka plan deseni ayarlama.
            style.Pattern = BackgroundType.Solid;

            // Yeni Stil Bayrağı.
            StyleFlag styleFlag = new StyleFlag();

            // Tüm Stilleri Ayarla.
            styleFlag.All = true;

            // İlk on sütunun varsayılan genişliğini değiştir
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // Varsayılan olmayan biçimlendirmeye sahip Column nesnesini al
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // İlk on Column'a Stil uygula
                column.ApplyStyle(style, styleFlag);
            }

            // Excel dosyasını kaydetme
            workbook.Save("ColumnCollectionExample.xlsx");
            workbook.Save("ColumnCollectionExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Column](../column/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


