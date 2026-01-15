---
title: Class ConnectionParameterCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalConnections.ConnectionParameterCollection class. Specifies the ConnectionParameter collection
type: docs
url: /net/aspose.cells.externalconnections/connectionparametercollection/
---
## ConnectionParameterCollection class

Specifies the [`ConnectionParameter`](../connectionparameter/) collection

```csharp
public class ConnectionParameterCollection : CollectionBase<ConnectionParameter>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/connectionparametercollection/item/) { get; } | Gets the [`ConnectionParameter`](../connectionparameter/) element at the specified index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConnectionParameter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConnectionParameter, IComparer&lt;ConnectionParameter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConnectionParameter, IComparer&lt;ConnectionParameter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConnectionParameter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConnectionParameter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConnectionParameter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConnectionParameter[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConnectionParameter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterCollectionDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Get the first external connection (will create one if none exists)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Get the parameters collection from the connection
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Demonstrate basic functionality by checking collection properties
                Console.WriteLine($"ConnectionParameterCollection count: {parameters.Count}");
                
                // Attempt to access an item (will be null if collection is empty)
                if (parameters.Count > 0)
                {
                    ConnectionParameter param = parameters[0];
                    Console.WriteLine(param == null ? "No parameters in collection" : "Parameter exists");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Save the workbook
                workbook.Save("ConnectionParameterCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameterCollection: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ConnectionParameter](../connectionparameter/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


