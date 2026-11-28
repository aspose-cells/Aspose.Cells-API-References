---
title: "Sınıf ListColumnCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.ListColumnCollection sınıfı. Tablo içindeki tüm ListColumn nesnelerinin bir listesini temsil eder"
type: docs
url: /tr/net/aspose.cells.tables/listcolumncollection/
---
## ListColumnCollection class

Tablodaki tüm [`ListColumn`](../listcolumn/) nesnelerinin bir listesini temsil eder.

```csharp
public class ListColumnCollection : CollectionBase<ListColumn>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listcolumncollection/item/) { get; } | İndeksle ListColumn'u alır. (2 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ListColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ListColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ListColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ListColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int, int) |  |
| [RemoveAt](../../aspose.cells.tables/listcolumncollection/removeat/#removeat)(int) | İndeksle [`ListColumn`](../listcolumn/) kaldır. (2 yöntem) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnCollectionDemo
    {
        public static void ListColumnCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Çalışma sayfasını bazı verilerle doldurun
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Çalışma sayfasına bir ListObject (tablo) ekle
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // ListObject'in ListColumnCollection'ına eriş
            ListColumnCollection listColumns = table.ListColumns;

            // ListColumnCollection özelliklerine erişimi göster
            Console.WriteLine("Number of columns in the table: " + listColumns.Count);

            // İndeksle bireysel ListColumn'a eriş
            ListColumn firstColumn = listColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);

            // ListColumnCollection'ın kapasitesini değiştir
            listColumns.Capacity = 10;
            Console.WriteLine("New capacity of the ListColumnCollection: " + listColumns.Capacity);

            // Çalışma kitabını kaydedin
            workbook.Save("ListColumnCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListColumn](../listcolumn/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


