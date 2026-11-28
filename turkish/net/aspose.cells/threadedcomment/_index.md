---
title: "Sınıf ThreadedComment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ThreadedComment sınıfı. İş parçacıklı yorumu temsil eder"
type: docs
url: /tr/net/aspose.cells/threadedcomment/
---
## ThreadedComment class

Konulu yorumu temsil eder.

```csharp
public class ThreadedComment
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Yorumun yazarını alır. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Yorumun sütun indeksini alır. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Bu iş parçacıklı yorumun oluşturulma zamanını alır ve ayarlar. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Yorumun metnini alır ve ayarlar. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Yorumun satır indeksini alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma kitabına yazarları ekle
            int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
            int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
            
            // Yazar referanslarını al
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
            
            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Yoruma iş parçacıklı yorum ekle
            int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Ek özellikleri ayarla
            threadedComment.Notes = "Additional notes";
            
            // İş parçacıklı yoruma bir yanıt ekle
            int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
            ThreadedComment reply = comment.ThreadedComments[replyIndex];
            
            // Çalışma kitabını kaydedin
            workbook.Save("ThreadedCommentDemo.xlsx");
            
            Console.WriteLine("Threaded comment demo completed.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


