---
title: "Classe ExternalConnectionCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ExternalConnections.ExternalConnectionCollection. Specifica la raccolta ExternalConnection"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnectioncollection/
---
## ExternalConnectionCollection class

Specifica la raccolta [`ExternalConnection`](../externalconnection/)

```csharp
public class ExternalConnectionCollection : CollectionBase<ExternalConnection>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item/) { get; } | Ottiene l'elemento [`ExternalConnection`](../externalconnection/) all'indice specificato. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
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
| [GetExternalConnectionById](../../aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/)(int) | Ottiene l'elemento [`ExternalConnection`](../externalconnection/) con l'id specificato. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

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
            // Carica una cartella di lavoro esistente che contiene connessioni esterne
            Workbook workbook = new Workbook("ExternalConnectionCollectionExample_original.xlsx");

            // Ottieni la raccolta delle connessioni esterne dalla cartella di lavoro
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Itera attraverso le connessioni esterne e stampa i loro ID
            for (int i = 0; i < dataConns.Count; i++)
            {
                ExternalConnection dataConn = dataConns[i];
                // Ottieni l'ID della connessione esterna
                Console.WriteLine($"External Connection ID: {dataConn.ConnectionId}");
            }

            // Esempio di accesso a una specifica connessione esterna per ID
            int specificConnId = 1; // Example ID
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(specificConnId);
            if (specificConn != null)
            {
                Console.WriteLine($"Found External Connection with ID {specificConnId}");
                // Puoi accedere e modificare le proprietà della connessione specifica qui
                specificConn.Name = "Updated Connection Name";
            }

            // Salva la cartella di lavoro se sono state apportate modifiche
            workbook.Save("ExternalConnectionCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


