---
title: "WorksheetCollection.ThreadedCommentAuthors"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. İş parçacıklı yorum yazarlarının listesini alır"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/threadedcommentauthors/
---
## WorksheetCollection.ThreadedCommentAuthors property

İşlemeli yorum yazarlarının listesini alır.

```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyThreadedCommentAuthorsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir iş parçacıklı yorum yazarı ekle
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo", "DA");

            // Az önce eklediğimiz yazarı al
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // C2 hücresine iş parçacıklı yorumlar ekle
            AddThreadedComment(worksheet, "C2", "First comment", author);
            AddThreadedComment(worksheet, "C2", "Second comment", author);
            AddThreadedComment(worksheet, "C2", "Third comment", author);

            // Çalışma kitabını kaydedin
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }

        private static void AddThreadedComment(Worksheet worksheet, string cellName, string text, ThreadedCommentAuthor author)
        {
            // Yorumu eklemek istediğimiz hücreyi al
            Cell cell = worksheet.Cells[cellName];
            
            // Bir iş parçacıklı yorum ekle (void döndürür, ThreadedComment değil)
            worksheet.Comments.AddThreadedComment(cellName, text, author);
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


