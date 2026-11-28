---
title: "ThreadedCommentCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedCommentCollection özelliği. Belirli indeksle iş parçacıklı yorumu alır"
type: docs
url: /tr/net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

Belirli indeksle iş parçacıklı yorumu alır.

```csharp
public ThreadedComment this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir yorum ekle
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Initial comment";

            // İş parçacıklı yorumlar ekle
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Yazarları ekle
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // İş parçacıklı yorumlar ekle
            threadedComments.Add("Reply 1", authors[author1Index]);
            threadedComments.Add("Reply 2", authors[author2Index]);

            // Item özelliğinin kullanımını göster
            ThreadedComment firstComment = threadedComments[0];
            ThreadedComment secondComment = threadedComments[1];

            Console.WriteLine("First comment author: " + firstComment.Author.Name);
            Console.WriteLine("Second comment author: " + secondComment.Author.Name);

            // İkinci yorumun yazarını değiştir
            secondComment.Author = authors[author1Index];
            Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);

            // Çalışma kitabını kaydedin
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


