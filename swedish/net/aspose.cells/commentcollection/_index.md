---
title: "Klass CommentCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CommentCollection klass. Inkapslar en samling av Comment-objekt"
type: docs
url: /sv/net/aspose.cells/commentcollection/
---
## CommentCollection class

Inkapslar en samling av [`Comment`](../comment/) objekt.

```csharp
public class CommentCollection : CollectionBase<Comment>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/commentcollection/item/) { get; } | Hämtar [`Comment`](../comment/) elementet på det angivna indexet. (3 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/commentcollection/add/#add_1)(string) | Lägger till en kommentar i samlingen. |
| [Add](../../aspose.cells/commentcollection/add/#add)(int, int) | Lägger till en kommentar i samlingen. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment_1)(string, string, ThreadedCommentAuthor) | Lägger till en trådad kommentar. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment)(int, int, string, ThreadedCommentAuthor) | Lägger till en trådad kommentar. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment, IComparer&lt;Comment&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Comment, IComparer&lt;Comment&gt;) |  |
| [Clear](../../aspose.cells/commentcollection/clear/#clear)() | Tar bort alla kommentarer; (2 metoder) |
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
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments_1)(string) | Hämtar de trådade kommentarerna efter cellnamn. |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments)(int, int) | Hämtar de trådade kommentarerna efter rad- och kolumnindex. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_2)(string) | Tar bort kommentaren för den specifika cellen. |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_1)(int, int) | Tar bort kommentaren för den specifika cellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CommentCollectionDemo
    {
        public static void CommentCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till kommentarssamlingen i kalkylbladet
            CommentCollection comments = worksheet.Comments;

            // Lägg till en kommentar till cell A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Author = "Author1";
            comment1.Font.Name = "Times New Roman";

            // Lägg till en kommentar i cell B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";
            comment2.Author = "Author2";

            // Lägg till en trådad kommentar i cell C3
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Author3", "user3", "provider3");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            comments.AddThreadedComment(2, 2, "This is a threaded comment.", author);

            // Hämta trådade kommentarer från cell C3
            var threadedComments = comments.GetThreadedComments(2, 2);
            foreach (var threadedComment in threadedComments)
            {
                Console.WriteLine(threadedComment.Notes);
            }

            // Ta bort kommentaren i cell A1
            comments.RemoveAt(0, 0);

            // Rensa alla kommentarer
            comments.Clear();

            // Spara arbetsboken
            workbook.Save("CommentCollectionExample.xlsx");
            workbook.Save("CommentCollectionExample.pdf");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Comment](../comment/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


