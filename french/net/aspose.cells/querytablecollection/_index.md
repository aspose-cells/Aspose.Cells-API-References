---
title: "Classe QueryTableCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.QueryTableCollection. Une collection d'objets QueryTableCollection qui représentent les informations de la collection QueryTable"
type: docs
url: /fr/net/aspose.cells/querytablecollection/
---
## QueryTableCollection class

Une collection d'objets `QueryTableCollection` qui représentent les informations de la collection QueryTable.

```csharp
public class QueryTableCollection : CollectionBase<QueryTable>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/querytablecollection/item/) { get; } | Obtient la querytable à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
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

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionDemo
    {
        public static void QueryTableCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à la QueryTableCollection de la feuille de calcul
            QueryTableCollection queryTables = worksheet.QueryTables;
            
            // Affiche le nombre de QueryTables dans la feuille de calcul
            Console.WriteLine("Number of QueryTables: " + queryTables.Count);
            
            // Définissez la capacité de la QueryTableCollection
            queryTables.Capacity = 10;
            Console.WriteLine("Capacity of QueryTableCollection: " + queryTables.Capacity);
            
            // En supposant qu'il y ait au moins un QueryTable, accédez au premier QueryTable
            if (queryTables.Count > 0)
            {
                QueryTable queryTable = queryTables[0];
                Console.WriteLine("First QueryTable accessed.");
            }
            else
            {
                Console.WriteLine("No QueryTables found in the worksheet.");
            }
            
            // Enregistrez le classeur
            workbook.Save("QueryTableCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [QueryTable](../querytable/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


