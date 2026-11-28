---
title: "ThreadedCommentAuthorCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadedCommentAuthorCollection yöntemi. Bir konu yorumcusu ekler"
type: docs
url: /tr/net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

Bir iş parçacığı yorum kişisi ekler.

```csharp
public int Add(string name, string userId, string providerId)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Kişinin adı. |
| userId | String |  |
| providerId | String | Sağlayıcının kimliği |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir iş parçacıklı yorum yazarı ekle
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");

            // Eklenen yazarı al
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Yazarı kullanarak konu yorumları ekle
            worksheet.Comments.AddThreadedComment("C2", "First comment", author);
            worksheet.Comments.AddThreadedComment("C2", "Second comment", author);

            // Çalışma kitabını kaydedin
            workbook.Save("ThreadedCommentsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


