---
title: "ThreadedComment.CreatedTime"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedComment özelliği. Bu threaded comment'in oluşturulma zamanını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/threadedcomment/createdtime/
---
## ThreadedComment.CreatedTime property

Bu iş parçacıklı yorumun oluşturulma zamanını alır ve ayarlar.

```csharp
public DateTime CreatedTime { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir threaded comment yazarı oluşturun
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
            
            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // İşlemeli bir yorum ekle
            int threadedCommentIndex = comment.ThreadedComments.Add("Test comment", author);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // CreatedTime özelliğini gösterin
            Console.WriteLine("Threaded comment created at: " + threadedComment.CreatedTime);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


