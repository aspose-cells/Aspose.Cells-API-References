---
title: "Clase QueryTableCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.QueryTableCollection. Una colección de objetos QueryTableCollection que representan la información de la colección QueryTable"
type: docs
url: /es/net/aspose.cells/querytablecollection/
---
## QueryTableCollection class

Una colección de objetos `QueryTableCollection` que representan la información de la colección QueryTable.

```csharp
public class QueryTableCollection : CollectionBase<QueryTable>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/querytablecollection/item/) { get; } | Obtiene la querytable por el índice específico. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
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

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionDemo
    {
        public static void QueryTableCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo del libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda a la QueryTableCollection de la hoja de cálculo
            QueryTableCollection queryTables = worksheet.QueryTables;
            
            // Muestra el recuento de QueryTables en la hoja de cálculo
            Console.WriteLine("Number of QueryTables: " + queryTables.Count);
            
            // Establece la capacidad de la QueryTableCollection
            queryTables.Capacity = 10;
            Console.WriteLine("Capacity of QueryTableCollection: " + queryTables.Capacity);
            
            // Suponiendo que haya al menos una QueryTable, acceda a la primera QueryTable
            if (queryTables.Count > 0)
            {
                QueryTable queryTable = queryTables[0];
                Console.WriteLine("First QueryTable accessed.");
            }
            else
            {
                Console.WriteLine("No QueryTables found in the worksheet.");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("QueryTableCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [QueryTable](../querytable/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


