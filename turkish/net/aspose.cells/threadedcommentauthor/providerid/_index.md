---
title: "ThreadedCommentAuthor.ProviderId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedCommentAuthor özelliği. Sağlayıcının kimliğini alır"
type: docs
url: /tr/net/aspose.cells/threadedcommentauthor/providerid/
---
## ThreadedCommentAuthor.ProviderId property

Sağlayıcının kimliğini alır.

```csharp
public string ProviderId { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyProviderIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Bir threaded comment yazar ekleyin ve indeksini alın
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
                
                // ThreadedCommentAuthor nesnesini alın
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
                
                // ProviderId değerini göster (okuma işlemi)
                Console.WriteLine("Author ProviderId: " + author.ProviderId);
                
                // Yazarı kullanarak bir threaded comment oluşturun
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
                
                // Çalışma kitabını kaydedin
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
                
                Console.WriteLine("Demo completed successfully.");
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


