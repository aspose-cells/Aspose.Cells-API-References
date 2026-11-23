---
title: "Classe ListColumnCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Tables.ListColumnCollection. Représente une liste de tous les objets ListColumn dans le tableau"
type: docs
url: /fr/net/aspose.cells.tables/listcolumncollection/
---
## ListColumnCollection class

Représente une liste de tous les objets [`ListColumn`](../listcolumn/) dans le tableau.

```csharp
public class ListColumnCollection : CollectionBase<ListColumn>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/listcolumncollection/item/) { get; } | Obtient le ListColumn par l'index. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ListColumn, IComparer&lt;ListColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ListColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ListColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ListColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ListColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ListColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ListColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ListColumn&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ListColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ListColumn, int, int) |  |
| [RemoveAt](../../aspose.cells.tables/listcolumncollection/removeat/#removeat)(int) | Supprime le [`ListColumn`](../listcolumn/) par index. (2 méthodes) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnCollectionDemo
    {
        public static void ListColumnCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplissez la feuille de calcul avec quelques données
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Ajoutez un ListObject (table) à la feuille de calcul
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Accédez à la ListColumnCollection du ListObject
            ListColumnCollection listColumns = table.ListColumns;

            // Démontrer l'accès aux propriétés de ListColumnCollection
            Console.WriteLine("Number of columns in the table: " + listColumns.Count);

            // Accédez à un ListColumn individuel par index
            ListColumn firstColumn = listColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);

            // Modifiez la capacité de la ListColumnCollection
            listColumns.Capacity = 10;
            Console.WriteLine("New capacity of the ListColumnCollection: " + listColumns.Capacity);

            // Enregistrez le classeur
            workbook.Save("ListColumnCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ListColumn](../listcolumn/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


