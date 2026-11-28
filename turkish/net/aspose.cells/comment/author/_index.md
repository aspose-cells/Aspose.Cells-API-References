---
title: "Comment.Author"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Orijinal yorum yazarının adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/comment/author/
---
## Comment.Author property

Orijinal yorum yazarının adını alır ve ayarlar.

```csharp
public string Author { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Yorum yazarını ve notu ayarla
            comment.Author = "Carl.Yang";
            comment.Note = "This is a sample comment";

            // Yorum yazarını göster
            Console.WriteLine("Comment Author: " + comment.Author);
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


