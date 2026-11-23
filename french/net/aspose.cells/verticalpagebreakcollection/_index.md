---
title: "Classe VerticalPageBreakCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.VerticalPageBreakCollection. Encapsule une collection d'objets VerticalPageBreak"
type: docs
url: /fr/net/aspose.cells/verticalpagebreakcollection/
---
## VerticalPageBreakCollection class

Encapsule une collection d'objets [`VerticalPageBreak`](../verticalpagebreak/).

```csharp
public class VerticalPageBreakCollection : CollectionBase<VerticalPageBreak>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/verticalpagebreakcollection/item/) { get; } | Obtient l'élément [`VerticalPageBreak`](../verticalpagebreak/) à l'index spécifié. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add)(int) | Ajoute un saut de page vertical à la collection. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_3)(string) | Ajoute un saut de page vertical à la collection. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_1)(int, int) | Ajoute un saut de page vertical à la collection. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_2)(int, int, int) | Ajoute un saut de page vertical à la collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VerticalPageBreak) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VerticalPageBreak, IComparer&lt;VerticalPageBreak&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VerticalPageBreak, IComparer&lt;VerticalPageBreak&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VerticalPageBreak) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VerticalPageBreak[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VerticalPageBreak[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, VerticalPageBreak[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak, int, int) |  |
| [RemoveAt](../../aspose.cells/verticalpagebreakcollection/removeat/#removeat)(int) | Supprime l'élément VPageBreak à un nom spécifié. (2 méthodes) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionDemo
    {
        public static void VerticalPageBreakCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à la VerticalPageBreakCollection de la feuille de calcul
            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Ajouter des sauts de page verticaux
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3
            verticalPageBreaks.Add("G5"); // At cell G5

            // Supprimer un saut de page vertical à l'index 1
            verticalPageBreaks.RemoveAt(1);

            // Accéder et imprimer les détails des sauts de page verticaux
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");
            }

            // Enregistrez le classeur
            workbook.Save("VerticalPageBreakCollectionExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [VerticalPageBreak](../verticalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


