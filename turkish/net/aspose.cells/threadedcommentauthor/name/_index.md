---
title: "ThreadedCommentAuthor.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedCommentAuthor özelliği. Adı alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

Adı alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir yorum ve zincirli yorumlar ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            
            // Farklı yazarlarla zincirli yorumlar ekle
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // İş parçacıklı yorumlar ekle
            threadedComments.Add("Reply from User1", authors[author1Index]);
            threadedComments.Add("Reply from User2", authors[author2Index]);

            // Name özelliğinin kullanımını göster
            Console.WriteLine("First author name: " + threadedComments[0].Author.Name);
            Console.WriteLine("Second author name: " + threadedComments[1].Author.Name);

            // İkinci yorumun yazarını değiştir
            threadedComments[1].Author = authors[author1Index];
            Console.WriteLine("Updated second author name: " + threadedComments[1].Author.Name);

            // Çalışma kitabını kaydedin
            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


