---
title: "FilterColumnCollection sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FilterColumnCollection sınıfı. Otomatik filtrelenmiş bir aralıktaki tüm filtreleri temsil eden Filter nesnelerinin bir koleksiyonu"
type: docs
url: /tr/net/aspose.cells/filtercolumncollection/
---
## FilterColumnCollection class

Otomatik filtrelenmiş bir aralıktaki tüm filtreleri temsil eden Filter nesnelerinin bir koleksiyonu.

```csharp
public class FilterColumnCollection : CollectionBase<FilterColumn>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/filtercolumncollection/item/) { get; } | Özel alanda [`FilterColumn`](../filtercolumn/) nesnesini alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FilterColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FilterColumn, IComparer&lt;FilterColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FilterColumn, IComparer&lt;FilterColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FilterColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FilterColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FilterColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FilterColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FilterColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FilterColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FilterColumn&gt;) |  |
| [GetByIndex](../../aspose.cells/filtercolumncollection/getbyindex/)(int) | Bir koleksiyondan tek bir Filter nesnesi döndürür. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn, int, int) |  |
| [RemoveAt](../../aspose.cells/filtercolumncollection/removeat/#removeat)(int) | (2 yöntem) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnCollectionDemo
    {
        public static void FilterColumnCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Filtrelemek için bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(22);

            // Bir AutoFilter oluştur
            worksheet.AutoFilter.Range = "A1:B4";

            // FilterColumnCollection'ı al
            FilterColumnCollection filterColumns = worksheet.AutoFilter.FilterColumns;

            // İkinci sütuna (Yaş) bir filtre ekle
            worksheet.AutoFilter.AddFilter(1, "25");

            // Filtreyi uygula
            worksheet.AutoFilter.Refresh();

            // FilterColumnCollection'a erişin ve onu yönetin
            Console.WriteLine("Number of filters applied: " + filterColumns.Count);

            // İlk filtre sütununu alın
            FilterColumn filterColumn = filterColumns.GetByIndex(0);
            Console.WriteLine("Filter applied on column index: " + filterColumn.FieldIndex);

            // Filtreyi kaldır
            filterColumns.RemoveAt(0);
            worksheet.AutoFilter.Refresh();

            // Çalışma kitabını kaydedin
            workbook.Save("FilterColumnCollectionExample.xlsx");
            workbook.Save("FilterColumnCollectionExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [FilterColumn](../filtercolumn/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


