---
title: "ThreadedCommentAuthor.UserId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedCommentAuthor özelliği. Kullanıcının kimliğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Kullanıcının kimliğini alır ve ayarlar.

```csharp
public string UserId { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ad, userId ve providerId ile bir threaded comment yazar ekleyin
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // ThreadedCommentAuthor nesnesini alın
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // UserId değerini göster (okuma işlemi)
                Console.WriteLine("Author UserId: " + author.UserId);

                // Yeni bir UserId ayarlamayı göster (yazma işlemi)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // Yazarı kullanarak bir threaded comment oluşturun
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // Çalışma kitabını kaydedin
                workbook.Save("UserIdDemo.xlsx");

                Console.WriteLine("UserId property demonstration completed successfully.");
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


