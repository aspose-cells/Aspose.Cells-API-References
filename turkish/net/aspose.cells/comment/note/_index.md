---
title: "Comment.Note"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun içeriğini temsil eder"
type: docs
url: /tr/net/aspose.cells/comment/note/
---
## Comment.Note property

Yorumun içeriğini temsil eder.

```csharp
public string Note { get; set; }
```

### Açıklamalar

Bu bir zincirleme yorum ise, not değiştirilemez, aksi takdirde MS Excel bunu zincirleme yorum olarak işleyemez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            
            // Yorum için notu ayarla
            comment1.Note = "First note.";
            
            // Notun ayarlandığını doğrula
            Console.WriteLine("Comment note: " + comment1.Note);
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


