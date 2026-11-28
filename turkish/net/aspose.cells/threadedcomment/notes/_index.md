---
title: "ThreadedComment.Notes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedComment özelliği. Yorumun metnini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Yorumun metnini alır ve ayarlar.

```csharp
public string Notes { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir threaded comment yazarını oluşturun veya edinin
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // A1 hücresine (satır 0, sütun 0) başlangıç metniyle bir threaded comment ekleyin
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // Yeni eklenen threaded comment'i alın
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // Notes özelliğini güncelleyin (yorum metni)
                threadedComment.Notes = "Updated comment notes";

                // Notes özelliği değerini okuyun ve görüntüleyin
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // Çalışma kitabını kaydedin (isteğe bağlı)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
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


