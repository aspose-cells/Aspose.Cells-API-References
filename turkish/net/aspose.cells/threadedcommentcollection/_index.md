---
title: "ThreadedCommentCollection sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ThreadedCommentCollection sınıfı. İş parçacıklı yorumların listesini temsil eder"
type: docs
url: /tr/net/aspose.cells/threadedcommentcollection/
---
## ThreadedCommentCollection class

Konulu yorumların listesini temsil eder.

```csharp
public class ThreadedCommentCollection : CollectionBase<ThreadedComment>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/threadedcommentcollection/item/) { get; } | Belirli indeksle iş parçacıklı yorumu alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/threadedcommentcollection/add/)(string, ThreadedCommentAuthor) | Bir iş parçacıklı yorum ekler. |
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

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CommentCollection comments = worksheet.Comments;

            // İş parçacıklı yorumlar ekle
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo_user", "demo_provider");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            
            comments.AddThreadedComment(0, 0, "First threaded comment", author);
            comments.AddThreadedComment(0, 0, "Reply to first comment", author);

            // İş parçacıklı yorumları al
            var threadedComments = comments.GetThreadedComments(0, 0);
            Console.WriteLine("Threaded comments in cell A1:");
            foreach (var comment in threadedComments)
            {
                Console.WriteLine($"- {comment.Notes} (by {comment.Author.Name})");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ThreadedComment](../threadedcomment/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


