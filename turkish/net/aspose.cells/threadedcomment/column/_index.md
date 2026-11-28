---
title: "ThreadedComment.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedComment özelliği. Yorumun sütun indeksini alır"
type: docs
url: /tr/net/aspose.cells/threadedcomment/column/
---
## ThreadedComment.Column property

Yorumun sütun indeksini alır.

```csharp
public int Column { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // İlk olarak bir zincirli yorum yazarını oluşturun
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                
                // A1 hücresine (satır 0, sütun 0) bir threaded comment ekleyin
                int commentRow = 0;
                int commentColumn = 0;
                worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
                
                // İlk threaded comment'i alın
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Column özelliği değerini göster (yalnızca okunur)
                Console.WriteLine("Threaded comment column index: " + comment.Column);
                
                // Sütun indeksinin yorumun yerleştirildiği konumla eşleştiğini doğrula
                if (comment.Column == commentColumn)
                {
                    Console.WriteLine("Comment is correctly placed in column " + commentColumn);
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ThreadedCommentColumnDemo.xlsx");
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


