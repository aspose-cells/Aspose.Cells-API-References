---
title: "Class HorizontalPageBreakCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.HorizontalPageBreakCollection class. Incapsula una raccolta di oggetti HorizontalPageBreak"
type: docs
url: /it/net/aspose.cells/horizontalpagebreakcollection/
---
## HorizontalPageBreakCollection class

Incapsula una raccolta di oggetti [`HorizontalPageBreak`](../horizontalpagebreak/).

```csharp
public class HorizontalPageBreakCollection : CollectionBase<HorizontalPageBreak>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/horizontalpagebreakcollection/item/) { get; } | Ottiene l'elemento [`HorizontalPageBreak`](../horizontalpagebreak/) all'indice specificato. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add)(int) | Aggiunge un'interruzione di pagina orizzontale alla raccolta. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_3)(string) | Aggiunge un'interruzione di pagina orizzontale alla raccolta. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_1)(int, int) | Aggiunge un'interruzione di pagina orizzontale alla raccolta. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_2)(int, int, int) | Aggiunge un'interruzione di pagina orizzontale alla raccolta. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HorizontalPageBreak) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HorizontalPageBreak[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int, int) |  |
| [RemoveAt](../../aspose.cells/horizontalpagebreakcollection/removeat/#removeat)(int) | Rimuove l'elemento HPageBreak con un nome specificato. (2 metodi) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakCollectionDemo
    {
        public static void HorizontalPageBreakCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'interruzione di pagina orizzontale alla riga 5
            worksheet.HorizontalPageBreaks.Add(5);
            
            // Aggiungi un'interruzione di pagina orizzontale alla riga 10, dalla colonna 1 alla colonna 5
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            // Aggiungi un'interruzione di pagina orizzontale alla riga 15, a partire dalla colonna 2
            worksheet.HorizontalPageBreaks.Add(15, 2);
            
            // Aggiungi un'interruzione di pagina orizzontale alla cella "G5"
            worksheet.HorizontalPageBreaks.Add("G5");
            
            // Rimuovi la prima interruzione di pagina orizzontale
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Salva la cartella di lavoro
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
            workbook.Save("HorizontalPageBreakCollectionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HorizontalPageBreak](../horizontalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


