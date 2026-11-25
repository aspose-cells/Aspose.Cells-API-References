---
title: "Classe VerticalPageBreakCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.VerticalPageBreakCollection. Incapsula una collezione di oggetti VerticalPageBreak"
type: docs
url: /it/net/aspose.cells/verticalpagebreakcollection/
---
## VerticalPageBreakCollection class

Incapsula una collezione di oggetti [`VerticalPageBreak`](../verticalpagebreak/).

```csharp
public class VerticalPageBreakCollection : CollectionBase<VerticalPageBreak>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/verticalpagebreakcollection/item/) { get; } | Ottiene l'elemento [`VerticalPageBreak`](../verticalpagebreak/) all'indice specificato. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add)(int) | Aggiunge un'interruzione di pagina verticale alla collezione. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_3)(string) | Aggiunge un'interruzione di pagina verticale alla collezione. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_1)(int, int) | Aggiunge un'interruzione di pagina verticale alla collezione. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_2)(int, int, int) | Aggiunge un'interruzione di pagina verticale alla collezione. |
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
| [RemoveAt](../../aspose.cells/verticalpagebreakcollection/removeat/#removeat)(int) | Rimuove l'elemento VPageBreak con un nome specificato. (2 metodi) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionDemo
    {
        public static void VerticalPageBreakCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla VerticalPageBreakCollection del foglio di lavoro
            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Aggiungi interruzioni di pagina verticali
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3
            verticalPageBreaks.Add("G5"); // At cell G5

            // Rimuovi un'interruzione di pagina verticale all'indice 1
            verticalPageBreaks.RemoveAt(1);

            // Accedi e stampa i dettagli delle interruzioni di pagina verticali
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");
            }

            // Salva la cartella di lavoro
            workbook.Save("VerticalPageBreakCollectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [VerticalPageBreak](../verticalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


