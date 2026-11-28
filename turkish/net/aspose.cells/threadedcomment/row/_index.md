---
title: "ThreadedComment.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedComment özelliği. Yorumun satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/threadedcomment/row/
---
## ThreadedComment.Row property

Yorumun satır indeksini alır.

```csharp
public int Row { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Bir threaded comment yazarı oluşturun
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "Test Author";
                author.UserId = "test@example.com";
                
                // B2 hücresine (satır 1, sütun 1) bir threaded comment ekleyin
                worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
                
                // İlk threaded comment'i alın
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Row özelliği değerini görüntüleyin (yalnızca okuma)
                Console.WriteLine("Threaded comment row index: " + comment.Row);
                
                // Satır indeksinin yorumun yerleştirildiği konumla eşleştiğini doğrulayın
                if (comment.Row == 1)
                {
                    Console.WriteLine("Comment is correctly placed in row 1");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ThreadedCommentRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


