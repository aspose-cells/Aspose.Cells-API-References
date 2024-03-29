---
title: ExternalConnectionCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Specifica ilExternalConnection./externalconnection collezione
type: docs
weight: 3300
url: /it/net/aspose.cells.externalconnections/externalconnectioncollection/
---
## ExternalConnectionCollection class

Specifica il[`ExternalConnection`](../externalconnection) collezione

```csharp
public class ExternalConnectionCollection : CollectionBase<ExternalConnection>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item) { get; set; } | Ottiene il[`ExternalConnection`](../externalconnection) elemento all'indice specificato. (2 indexers) |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item) { get; } | Ottiene il[`ExternalConnection`](../externalconnection) elemento con il nome specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ExternalConnection) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ExternalConnection, IComparer&lt;ExternalConnection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, ExternalConnection, IComparer&lt;ExternalConnection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(ExternalConnection) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ExternalConnection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ExternalConnection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, ExternalConnection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;ExternalConnection&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;ExternalConnection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;ExternalConnection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetExternalConnectionById](../../aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid)(int) | Ottiene il[`ExternalConnection`](../externalconnection) elemento con l'id. specificato |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ExternalConnection) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ExternalConnection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ExternalConnection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ExternalConnection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ExternalConnection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ExternalConnection, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Esempi

```csharp
[C#]
Workbook wb = new Workbook("connection.xlsx");
ExternalConnectionCollection dataConns = wb.DataConnections;
ExternalConnection dataConn = null;
for (int i = 0; i < dataConns.Count; i++)
{
    dataConn = dataConns[i];
    //ottieni l'ID della connessione esterna
    Console.WriteLine(dataConn.ConnectionId);
}

[Visual Basic]
Dim wb As Workbook = New Workbook("connection.xlsx")
Dim dataConns As ExternalConnectionCollection = wb.DataConnections
Dim dataConn As ExternalConnection
Dim count As Integer = dataConns.Count - 1
Dim i As Integer
For i = 0 To count Step 1
    dataConn = dataConns(i)
    'ottenere l'ID della connessione esterna
    Console.WriteLine(dataConn.ConnectionId)
Next
```

### Guarda anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [ExternalConnection](../externalconnection)
* spazio dei nomi [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
