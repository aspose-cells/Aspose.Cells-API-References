---
title: "Sınıf CommentCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CommentCollection sınıfı. Comment nesnelerinden oluşan bir koleksiyonu kapsar"
type: docs
url: /tr/net/aspose.cells/commentcollection/
---
## CommentCollection class

Bir [`Comment`](../comment/) nesnesi koleksiyonunu kapsar.

```csharp
public class CommentCollection : CollectionBase<Comment>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/commentcollection/item/) { get; } | Belirtilen indeksteki [`Comment`](../comment/) öğesini alır. (3 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/commentcollection/add/#add_1)(string) | Koleksiyona bir yorum ekler. |
| [Add](../../aspose.cells/commentcollection/add/#add)(int, int) | Koleksiyona bir yorum ekler. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment_1)(string, string, ThreadedCommentAuthor) | Bir iş parçacıklı yorum ekler. |
| [AddThreadedComment](../../aspose.cells/commentcollection/addthreadedcomment/#addthreadedcomment)(int, int, string, ThreadedCommentAuthor) | Bir iş parçacıklı yorum ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Comment, IComparer&lt;Comment&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Comment, IComparer&lt;Comment&gt;) |  |
| [Clear](../../aspose.cells/commentcollection/clear/#clear)() | Tüm yorumları kaldırır; (2 yöntem) |
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
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments_1)(string) | Hücre adıyla iş parçacıklı yorumları alır. |
| [GetThreadedComments](../../aspose.cells/commentcollection/getthreadedcomments/#getthreadedcomments)(int, int) | Satır ve sütun indeksine göre iş parçacıklı yorumları alır. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Comment, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Comment, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_2)(string) | Belirli hücrenin yorumunu kaldırır. |
| [RemoveAt](../../aspose.cells/commentcollection/removeat/#removeat_1)(int, int) | Belirli hücrenin yorumunu kaldırır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CommentCollectionDemo
    {
        public static void CommentCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının yorumlar koleksiyonuna erişin
            CommentCollection comments = worksheet.Comments;

            // A1 hücresine bir yorum ekle
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Author = "Author1";
            comment1.Font.Name = "Times New Roman";

            // B2 hücresine bir yorum ekleyin
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";
            comment2.Author = "Author2";

            // C3 hücresine bir iş parçacıklı yorum ekle
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Author3", "user3", "provider3");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            comments.AddThreadedComment(2, 2, "This is a threaded comment.", author);

            // C3 hücresinden iş parçacıklı yorumları al
            var threadedComments = comments.GetThreadedComments(2, 2);
            foreach (var threadedComment in threadedComments)
            {
                Console.WriteLine(threadedComment.Notes);
            }

            // A1 hücresindeki yorumu kaldır
            comments.RemoveAt(0, 0);

            // Tüm yorumları temizle
            comments.Clear();

            // Çalışma kitabını kaydedin
            workbook.Save("CommentCollectionExample.xlsx");
            workbook.Save("CommentCollectionExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Comment](../comment/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


