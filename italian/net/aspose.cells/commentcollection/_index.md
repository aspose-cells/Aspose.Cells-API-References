---
title: "Classe CommentCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CommentCollection. Incapsula una collezione di oggetti Comment"
type: docs
url: /it/net/aspose.cells/commentcollection/
---
## CommentCollection class

Incapsula una collezione di oggetti [`Comment`](../comment/).

```csharp
public class CommentCollection : CollectionBase<Comment>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/commentcollection/item/) { get; } | Restituisce l'elemento [`Comment`](../comment/) all'indice specificato. (3 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/commentcollection/add/#add_1)(string) | Aggiunge un commento alla collezione. |
| [Add](../../aspose.cells/commentcollection/add/#add)(int, int) | Aggiunge un commento alla collezione. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment_1)(string, string, ThreadedCommentAuthor) | Aggiunge un commento a thread. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment)(int, int, string, ThreadedCommentAuthor) | Aggiunge un commento a thread. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment, IComparer&lt;Comment&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Comment, IComparer&lt;Comment&gt;) |  |
| [Clear](../../aspose.cells/commentcollection/clear/#clear)() | Rimuove tutti i commenti; (2 metodi) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Comment) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Comment[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Comment[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Comment[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Comment&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Comment&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Comment&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Comment&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments_1)(string) | Restituisce i commenti in thread per nome della cella. |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments)(int, int) | Restituisce i commenti in thread per indice di riga e colonna. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_2)(string) | Rimuove il commento della cella specifica. |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_1)(int, int) | Rimuove il commento della cella specifica. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CommentCollectionDemo
    {
        public static void CommentCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla raccolta dei commenti del foglio di lavoro
            CommentCollection comments = worksheet.Comments;

            // Aggiungi un commento alla cella A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Author = "Author1";
            comment1.Font.Name = "Times New Roman";

            // Aggiungi un commento alla cella B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";
            comment2.Author = "Author2";

            // Aggiungi un commento in thread alla cella C3
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Author3", "user3", "provider3");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            comments.AddThreadedComment(2, 2, "This is a threaded comment.", author);

            // Recupera i commenti in thread dalla cella C3
            var threadedComments = comments.GetThreadedComments(2, 2);
            foreach (var threadedComment in threadedComments)
            {
                Console.WriteLine(threadedComment.Notes);
            }

            // Rimuovi il commento nella cella A1
            comments.RemoveAt(0, 0);

            // Cancella tutti i commenti
            comments.Clear();

            // Salva la cartella di lavoro
            workbook.Save("CommentCollectionExample.xlsx");
            workbook.Save("CommentCollectionExample.pdf");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Comment](../comment/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


