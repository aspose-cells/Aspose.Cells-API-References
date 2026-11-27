---
title: "Klass ExternalConnectionCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.ExternalConnectionCollection‑klass. Anger ExternalConnection‑samlingen"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnectioncollection/
---
## ExternalConnectionCollection class

Anger [`ExternalConnection`](../externalconnection/)-samlingen

```csharp
public class ExternalConnectionCollection : CollectionBase<ExternalConnection>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item/) { get; } | Hämtar [`ExternalConnection`](../externalconnection/)‑elementet på det angivna indexet. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
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
| [GetExternalConnectionById](../../aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/)(int) | Hämtar [`ExternalConnection`](../externalconnection/)‑elementet med det angivna id‑värdet. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

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
            // Läs in en befintlig arbetsbok som innehåller externa anslutningar
            Workbook workbook = new Workbook("ExternalConnectionCollectionExample_original.xlsx");

            // Hämta samlingen av externa anslutningar från arbetsboken
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Iterera genom de externa anslutningarna och skriv ut deras ID:n
            for (int i = 0; i < dataConns.Count; i++)
            {
                ExternalConnection dataConn = dataConns[i];
                // Hämta extern anslutnings‑ID
                Console.WriteLine($"External Connection ID: {dataConn.ConnectionId}");
            }

            // Exempel på hur man får åtkomst till en specifik extern anslutning via ID
            int specificConnId = 1; // Example ID
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(specificConnId);
            if (specificConn != null)
            {
                Console.WriteLine($"Found External Connection with ID {specificConnId}");
                // Du kan komma åt och ändra egenskaper för den specifika anslutningen här
                specificConn.Name = "Updated Connection Name";
            }

            // Spara arbetsboken om några ändringar har gjorts
            workbook.Save("ExternalConnectionCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


