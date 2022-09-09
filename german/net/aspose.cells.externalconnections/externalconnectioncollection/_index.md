---
title: ExternalConnectionCollection
second_title: Aspose.Cells für .NET-API-Referenz
description: Gibt die anExternalConnection./externalconnection Sammlung
type: docs
weight: 3300
url: /de/net/aspose.cells.externalconnections/externalconnectioncollection/
---
## ExternalConnectionCollection class

Gibt die an[`ExternalConnection`](../externalconnection) Sammlung

```csharp
public class ExternalConnectionCollection : CollectionBase<ExternalConnection>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item) { get; set; } | Ruft die ab[`ExternalConnection`](../externalconnection) Element am angegebenen Index. (2 indexers) |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item) { get; } | Ruft die ab[`ExternalConnection`](../externalconnection) Element mit dem angegebenen Namen. |

## Methoden

| Name | Beschreibung |
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
| [GetExternalConnectionById](../../aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid)(int) | Ruft die ab[`ExternalConnection`](../externalconnection) Element mit der angegebenen ID. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ExternalConnection) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ExternalConnection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ExternalConnection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ExternalConnection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ExternalConnection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ExternalConnection, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Beispiele

```csharp
[C#]
Workbook wb = new Workbook("connection.xlsx");
ExternalConnectionCollection dataConns = wb.DataConnections;
ExternalConnection dataConn = null;
for (int i = 0; i < dataConns.Count; i++)
{
    dataConn = dataConns[i];
    //Externe Verbindungs-ID abrufen
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
    'Externe Verbindungs-ID erhalten
    Console.WriteLine(dataConn.ConnectionId)
Next
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [ExternalConnection](../externalconnection)
* namensraum [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->