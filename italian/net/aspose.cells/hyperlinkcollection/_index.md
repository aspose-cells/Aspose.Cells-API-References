---
title: "Classe HyperlinkCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.HyperlinkCollection. Incapsula una collezione di oggetti Hyperlink."
type: docs
url: /it/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Incapsula una collezione di oggetti [`Hyperlink`](../hyperlink/).

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item/) { get; } | Ottiene l'elemento [`Hyperlink`](../hyperlink/) all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_1)(string, int, int, string) | Aggiunge un hyperlink a una cella specificata o a un intervallo di celle. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add)(int, int, int, int, string) | Aggiunge un hyperlink a una cella specificata o a un intervallo di celle. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_2)(string, string, string, string, string) | Aggiunge un hyperlink a una cella specificata o a un intervallo di celle. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear/#clear)() | Cancella tutti gli hyperlink. (2 metodi) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat/#removeat)(int) | Rimuove l'hyperlink all'indice specificato in questa collezione. (2 metodi) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkCollectionDemo
    {
        public static void HyperlinkCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di Hyperlink
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Aggiunta di un collegamento ipertestuale a un URL nella cella "A1"
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Aggiunta di un altro collegamento ipertestuale a un URL nella cella "B1"
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // Aggiunta di un collegamento ipertestuale con un intervallo di celle
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // Aggiunta di un collegamento ipertestuale con un testo specifico da visualizzare e suggerimento
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // Rimozione del primo collegamento ipertestuale
            hyperlinks.RemoveAt(0);

            // Cancellazione di tutti i collegamenti ipertestuali
            hyperlinks.Clear();

            // Aggiunta di nuovo di un collegamento ipertestuale per dimostrare il salvataggio
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Salvataggio del file Excel
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


