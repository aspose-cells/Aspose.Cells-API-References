---
title: Class ExternalConnectionCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalConnections.ExternalConnectionCollection class. Specifies the ExternalConnection collection
type: docs
url: /net/aspose.cells.externalconnections/externalconnectioncollection/
---
## ExternalConnectionCollection class

Specifies the [`ExternalConnection`](../externalconnection/) collection

```csharp
public class ExternalConnectionCollection : CollectionBase<ExternalConnection>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/externalconnectioncollection/item/) { get; } | Gets the [`ExternalConnection`](../externalconnection/) element at the specified index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
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
| [GetExternalConnectionById](../../aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/)(int) | Gets the [`ExternalConnection`](../externalconnection/) element with the specified id. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ExternalConnection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ExternalConnection, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

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
            // Load an existing workbook that contains external connections
            Workbook workbook = new Workbook("ExternalConnectionCollectionExample_original.xlsx");

            // Get the external connection collection from the workbook
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Iterate through the external connections and print their IDs
            for (int i = 0; i < dataConns.Count; i++)
            {
                ExternalConnection dataConn = dataConns[i];
                // Get external connection id
                Console.WriteLine($"External Connection ID: {dataConn.ConnectionId}");
            }

            // Example of accessing a specific external connection by ID
            int specificConnId = 1; // Example ID
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(specificConnId);
            if (specificConn != null)
            {
                Console.WriteLine($"Found External Connection with ID {specificConnId}");
                // You can access and modify properties of the specific connection here
                specificConn.Name = "Updated Connection Name";
            }

            // Save the workbook if any changes were made
            workbook.Save("ExternalConnectionCollectionExample.xlsx");
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


