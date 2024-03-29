---
title: CommentCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula una raccolta diComment./comment oggetti.
type: docs
weight: 1090
url: /it/net/aspose.cells/commentcollection/
---
## CommentCollection class

Incapsula una raccolta di[`Comment`](../comment) oggetti.

```csharp
public class CommentCollection : CollectionBase<Comment>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/commentcollection/item) { get; } | Ottiene il[`Comment`](../comment) elemento all'indice specificato. (3 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/commentcollection/add#add_1)(string) | Aggiunge un commento alla raccolta. |
| [Add](../../aspose.cells/commentcollection/add#add)(int, int) | Aggiunge un commento alla raccolta. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment#addthreadedcomment_1)(string, string, ThreadedCommentAuthor) | Aggiunge un commento in thread. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment#addthreadedcomment)(int, int, string, ThreadedCommentAuthor) | Aggiunge un commento in thread. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Comment) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Comment, IComparer&lt;Comment&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Comment, IComparer&lt;Comment&gt;) |  |
| [Clear](../../aspose.cells/commentcollection/clear#clear)() | Rimuove tutti i commenti; (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Comment) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Comment[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Comment[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Comment[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Comment&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Comment&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Comment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Comment&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Comment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Comment&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments#getthreadedcomments_1)(string) | Ottiene i commenti in thread in base al nome della cella. |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments#getthreadedcomments)(int, int) | Ottiene i commenti in thread per riga e indice di colonna. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Comment) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Comment, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Comment, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Comment) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Comment, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Comment, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |
| [RemoveAt](../../aspose.cells/commentcollection/removeat#removeat_2)(string) | Rimuove il commento della cella specifica. |
| [RemoveAt](../../aspose.cells/commentcollection/removeat#removeat_1)(int, int) | Rimuove il commento della cella specifica. |

### Esempi

```csharp
[C#]

Workbook workbook = new Workbook();

CommentCollection comments = workbook.Worksheets[0].Comments;

//fai i tuoi affari

[Visual Basic]

Dim workbook as Workbook = new Workbook()

Dim comments as CommentCollection = workbook.Worksheets(0).Comments
```

### Guarda anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Comment](../comment)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
