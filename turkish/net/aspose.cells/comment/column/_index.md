---
title: "Comment.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun sütun indeksini alır."
type: docs
url: /tr/net/aspose.cells/comment/column/
---
## Comment.Column property

Yorumun sütun indeksini alır.

```csharp
public int Column { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // B5 hücresine (sütun indeksi 1) bir yorum ekle
            int commentRow = 4;
            int commentColumn = 1;
            Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];

            // Yorum metnini ayarla
            comment.Note = "This is a sample comment";

            // Column özelliğinin kullanımını gösterin
            Console.WriteLine("Comment is in column: " + comment.Column);

            // Sütun indeksinin yerleştirdiğimiz konumla eşleştiğini doğrula
            if (comment.Column == commentColumn)
            {
                Console.WriteLine("Column property correctly returns the comment's column index");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


