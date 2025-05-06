---
title: Class ThreadedCommentCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThreadedCommentCollection class. Represents the list of threaded comments
type: docs
url: /net/aspose.cells/threadedcommentcollection/
---
## ThreadedCommentCollection class

Represents the list of threaded comments.

```csharp
public class ThreadedCommentCollection : CollectionBase<ThreadedComment>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/threadedcommentcollection/item/) { get; } | Gets the threaded comment by the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/threadedcommentcollection/add/)(string, ThreadedCommentAuthor) | Adds a threaded comment; |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ThreadedComment) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ThreadedComment, IComparer&lt;ThreadedComment&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ThreadedComment, IComparer&lt;ThreadedComment&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ThreadedComment) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ThreadedComment[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ThreadedComment[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ThreadedComment[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ThreadedComment&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ThreadedComment&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ThreadedComment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ThreadedComment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ThreadedComment&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ThreadedComment&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ThreadedComment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ThreadedComment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ThreadedComment&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ThreadedComment&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedComment) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedComment, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ThreadedComment, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedComment) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedComment, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ThreadedComment, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: var threadedComments = comments.GetThreadedComments(2, 2);
public static void Type_ThreadedCommentCollection()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the comments collection of the worksheet
            CommentCollection comments = worksheet.Comments;

            // Add a comment to cell A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = &quot;First note.&quot;;
            comment1.Author = &quot;Author1&quot;;
            comment1.Font.Name = &quot;Times New Roman&quot;;

            // Add a comment to cell B2
            comments.Add(&quot;B2&quot;);
            Comment comment2 = comments[&quot;B2&quot;];
            comment2.Note = &quot;Second note.&quot;;
            comment2.Author = &quot;Author2&quot;;

            // Add a threaded comment to cell C3
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add(&quot;Author3&quot;, &quot;user3&quot;, &quot;provider3&quot;);
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            comments.AddThreadedComment(2, 2, &quot;This is a threaded comment.&quot;, author);

            // Retrieve threaded comments from cell C3
            var threadedComments = comments.GetThreadedComments(2, 2);
            foreach (var threadedComment in threadedComments)
            {
                Console.WriteLine(threadedComment.Notes);
            }

            // Remove the comment at cell A1
            comments.RemoveAt(0, 0);

            // Clear all comments
            comments.Clear();

            // Save the workbook
            workbook.Save(&quot;CommentCollectionExample.xlsx&quot;);
            workbook.Save(&quot;CommentCollectionExample.pdf&quot;);
        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ThreadedComment](../threadedcomment/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


