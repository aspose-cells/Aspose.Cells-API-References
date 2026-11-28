---
title: "Sınıf ExternalConnectionCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.ExternalConnectionCollection sınıfı. ExternalConnection koleksiyonunu belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnectioncollection/
---
## ExternalConnectionCollection class

[`ExternalConnection`](../externalconnection/) koleksiyonunu belirtir

```csharp
public class ExternalConnectionCollection : CollectionBase<ExternalConnection>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item/) { get; } | Belirtilen indeksteki [`ExternalConnection`](../externalconnection/) öğesini alır. (2 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ExternalConnection) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ExternalConnection, IComparer&lt;ExternalConnection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ExternalConnection, IComparer&lt;ExternalConnection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ExternalConnection) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ExternalConnection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ExternalConnection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ExternalConnection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ExternalConnection&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ExternalConnection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetExternalConnectionById](../../aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/)(int) | Belirtilen kimliğe sahip [`ExternalConnection`](../externalconnection/) öğesini alır. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionDemo
    {
        public static void ExternalConnectionCollectionExample()
        {
            // Dış bağlantılar içeren mevcut bir çalışma kitabını yükle
            Workbook workbook = new Workbook("ExternalConnectionCollectionExample_original.xlsx");

            // Çalışma kitabından dış bağlantı koleksiyonunu al
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Dış bağlantılar arasında döngü yap ve kimliklerini (ID) yazdır
            for (int i = 0; i < dataConns.Count; i++)
            {
                ExternalConnection dataConn = dataConns[i];
                // Dış bağlantı kimliğini al
                Console.WriteLine($"External Connection ID: {dataConn.ConnectionId}");
            }

            // ID ile belirli bir dış bağlantıya erişme örneği
            int specificConnId = 1; // Example ID
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(specificConnId);
            if (specificConn != null)
            {
                Console.WriteLine($"Found External Connection with ID {specificConnId}");
                // Burada belirli bağlantının özelliklerine erişebilir ve bunları değiştirebilirsiniz
                specificConn.Name = "Updated Connection Name";
            }

            // Herhangi bir değişiklik yapıldıysa çalışma kitabını kaydet
            workbook.Save("ExternalConnectionCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


