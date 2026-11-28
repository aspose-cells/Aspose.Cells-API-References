---
title: "Sınıf QueryTableCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.QueryTableCollection sınıfı. QueryTable koleksiyonu bilgilerini temsil eden QueryTableCollection nesnelerinin bir koleksiyonu"
type: docs
url: /tr/net/aspose.cells/querytablecollection/
---
## QueryTableCollection class

`QueryTableCollection` nesnelerinin, QueryTable koleksiyonu bilgilerini temsil eden bir koleksiyonu.

```csharp
public class QueryTableCollection : CollectionBase<QueryTable>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/querytablecollection/item/) { get; } | Belirli bir indeksle QueryTable'ı alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(QueryTable) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(QueryTable, IComparer&lt;QueryTable&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, QueryTable, IComparer&lt;QueryTable&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(QueryTable) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(QueryTable[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(QueryTable[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, QueryTable[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;QueryTable&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;QueryTable&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;QueryTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;QueryTable&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;QueryTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;QueryTable&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(QueryTable, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(QueryTable, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionDemo
    {
        public static void QueryTableCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabındaki ilk çalışma sayfasına erişin
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasının QueryTableCollection'ına erişin
            QueryTableCollection queryTables = worksheet.QueryTables;
            
            // Çalışma sayfasındaki QueryTable'ların sayısını göster
            Console.WriteLine("Number of QueryTables: " + queryTables.Count);
            
            // QueryTableCollection'ın kapasitesini ayarla
            queryTables.Capacity = 10;
            Console.WriteLine("Capacity of QueryTableCollection: " + queryTables.Capacity);
            
            // En az bir QueryTable olduğu varsayılırsa, ilk QueryTable'a erişin
            if (queryTables.Count > 0)
            {
                QueryTable queryTable = queryTables[0];
                Console.WriteLine("First QueryTable accessed.");
            }
            else
            {
                Console.WriteLine("No QueryTables found in the worksheet.");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("QueryTableCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [QueryTable](../querytable/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


