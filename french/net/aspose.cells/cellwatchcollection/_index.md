---
title: "Classe CellWatchCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CellWatchCollection. Représente la collection de cellules de cette feuille de calcul surveillées dans la fenêtre de surveillance"
type: docs
url: /fr/net/aspose.cells/cellwatchcollection/
---
## CellWatchCollection class

Représente la collection de cellules de cette feuille de calcul surveillées dans la 'fenêtre de surveillance'.

```csharp
public class CellWatchCollection : CollectionBase<CellWatch>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CellWatchCollection](cellwatchcollection/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/cellwatchcollection/item/) { get; } | Obtient et définit [`CellWatch`](../cellwatch/) par index. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/cellwatchcollection/add/#add_1)(string) | Ajoute [`CellWatch`](../cellwatch/) avec le nom de la cellule. |
| [Add](../../aspose.cells/cellwatchcollection/add/#add)(int, int) | Ajoute [`CellWatch`](../cellwatch/) avec une ligne et une colonne. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CellWatch, IComparer&lt;CellWatch&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CellWatch) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CellWatch[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CellWatch[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CellWatch&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CellWatch&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CellWatch&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CellWatch&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CellWatch, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CellWatch, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionDemo
    {
        public static void CellWatchCollectionExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            
            // Obtenir la première Worksheet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez l'élément Cell Watch dans la fenêtre de surveillance
            int watchIndex = sheet.CellWatches.Add("B2");
            
            // Accéder à la CellWatchCollection
            CellWatchCollection cellWatches = sheet.CellWatches;
            
            // Accéder à l'élément CellWatch ajouté
            CellWatch cellWatch = cellWatches[watchIndex];
            
            // Afficher les propriétés de l'élément CellWatch
            Console.WriteLine("Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Modifier les propriétés de l'élément CellWatch
            cellWatch.Row = 1;
            cellWatch.Column = 1;
            cellWatch.CellName = "A2";
            
            // Afficher les propriétés modifiées de l'élément CellWatch
            Console.WriteLine("Modified Cell Watch Details:");
            Console.WriteLine($"Row: {cellWatch.Row}");
            Console.WriteLine($"Column: {cellWatch.Column}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            
            // Enregistrez le classeur
            workbook.Save("CellWatchCollectionExample.xlsx");
            workbook.Save("CellWatchCollectionExample.pdf");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CellWatch](../cellwatch/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


