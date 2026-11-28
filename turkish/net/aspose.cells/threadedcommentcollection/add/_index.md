---
title: "ThreadedCommentCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedCommentCollection yöntemi. Bir iş parçacıklı yorum ekler"
type: docs
url: /tr/net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Bir iş parçacıklı yorum ekler.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | İş parçacıklı yorumun metni. |
| yazar | ThreadedCommentAuthor | İş parçacıklı yorumun yazarı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // **ThreadedCommentAuthorCollection** kullanarak bir iş parçacıklı yorum yazarı oluşturun
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // Bir hücrenin iş parçacıklı yorumlar koleksiyonuna erişin
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // String ve ThreadedCommentAuthor parametreleriyle Add yöntemini çağırın
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // Sonucu göster
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // Çalışma kitabını kaydedin
                workbook.Save("ThreadedCommentAddDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


