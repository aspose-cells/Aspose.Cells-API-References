---
title: "ThreadedCommentAuthor sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ThreadedCommentAuthor sınıfı. İş parçacıklı yorumları oluşturan kişiyi temsil eder."
type: docs
url: /tr/net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Konulu yorumları oluşturan kişiyi temsil eder.

```csharp
public class ThreadedCommentAuthor
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Adı alır ve ayarlar. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Sağlayıcının kimliğini alır. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Kullanıcının kimliğini alır ve ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir yorum ekle
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // İşlemeli yorum yazarlarını ekle
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // İşlemeli bir yorum ekle
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Yazara eriş ve değiştir
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // Yeni bir yazar oluştur ve ata
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


