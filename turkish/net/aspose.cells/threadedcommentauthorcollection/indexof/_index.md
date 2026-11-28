---
title: "ThreadedCommentAuthorCollection.IndexOf"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedCommentAuthorCollection yöntemi. ThreadedCommentAuthor nesnesinin dizinini alır"
type: docs
url: /tr/net/aspose.cells/threadedcommentauthorcollection/indexof/
---
## ThreadedCommentAuthorCollection.IndexOf method

ThreadedCommentAuthor nesnesinin dizinini alır

```csharp
public int IndexOf(ThreadedCommentAuthor author)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yazar | ThreadedCommentAuthor | ThreadedCommentAuthor nesnesi |

### Dönüş Değeri

ThreadedCommentAuthor koleksiyonundaki dizin

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Dallanmış yorum yazarları koleksiyonunu alın
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Koleksiyona yazarlar ekleyin
            int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
            int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");

            // Yazar nesnelerini alın
            ThreadedCommentAuthor johnAuthor = authors[johnIndex];
            ThreadedCommentAuthor janeAuthor = authors[janeIndex];

            try
            {
                // Jane Smith'in konumunu bulmak için IndexOf yöntemini çağırın
                int foundIndex = authors.IndexOf(janeAuthor);
                
                // Sonucu göster
                Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");

                // Sonucun beklenen dizinle eşleştiğini doğrulayın
                if (foundIndex == janeIndex)
                {
                    Console.WriteLine("IndexOf result matches the expected index");
                }
                else
                {
                    Console.WriteLine("IndexOf result does not match the expected index");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


