---
title: "ThreadedComment.Author"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedComment özelliği. Yorumun yazarını alır"
type: docs
url: /tr/net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Yorumun yazarını alır.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma kitabından varsayılan threaded comment yazarını alın
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // A1 hücresine (satır 0, sütun 0) bir threaded comment ekleyin
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // İlk threaded comment'i alın
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // Author özelliği değerini görüntüleyin (okuma işlemi)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // Author özelliğini ayarlamayı gösterin (okuma/yazma olduğu için)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // Güncellenmiş Author özelliği değerini görüntüleyin
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // Çalışma kitabını kaydedin
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
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

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


