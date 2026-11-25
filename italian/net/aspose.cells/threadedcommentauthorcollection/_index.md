---
title: "Class ThreadedCommentAuthorCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ThreadedCommentAuthorCollection class. Rappresenta tutte le persone"
type: docs
url: /it/net/aspose.cells/threadedcommentauthorcollection/
---
## ThreadedCommentAuthorCollection class

Rappresenta tutte le persone.

```csharp
public class ThreadedCommentAuthorCollection : CollectionBase<ThreadedCommentAuthor>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ThreadedCommentAuthorCollection](threadedcommentauthorcollection/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CurrentPerson](../../aspose.cells/threadedcommentauthorcollection/currentperson/) { get; set; } | Ottiene e imposta l'utente corrente. |
| [Item](../../aspose.cells/threadedcommentauthorcollection/item/) { get; } | Ottiene la persona che crea i commenti in thread. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/threadedcommentauthorcollection/add/)(string, string, string) | Aggiunge una persona al commento in thread. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ThreadedCommentAuthor) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ThreadedCommentAuthor, IComparer&lt;ThreadedCommentAuthor&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ThreadedCommentAuthor, IComparer&lt;ThreadedCommentAuthor&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ThreadedCommentAuthor) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ThreadedCommentAuthor[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ThreadedCommentAuthor[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ThreadedCommentAuthor[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ThreadedCommentAuthor&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/threadedcommentauthorcollection/indexof/#indexof)(ThreadedCommentAuthor) | Ottiene l'indice dell'oggetto ThreadedCommentAuthor (2 metodi) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedCommentAuthor, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedCommentAuthor, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionDemo
    {
        public static void ThreadedCommentAuthorCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla ThreadedCommentAuthorCollection
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Aggiungi un nuovo autore di commenti in thread
            int authorIndex = authors.Add("John Doe", "john.doe@example.com", "providerId123");

            // Recupera l'autore aggiunto
            ThreadedCommentAuthor author = authors[authorIndex];

            // Imposta la persona corrente
            authors.CurrentPerson = author;

            // Visualizza i dettagli della persona corrente
            Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);

            // Salva la cartella di lavoro
            workbook.Save("ThreadedCommentAuthorCollectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ThreadedCommentAuthor](../threadedcommentauthor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


