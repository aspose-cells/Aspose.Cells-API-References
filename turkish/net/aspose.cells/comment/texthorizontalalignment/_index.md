---
title: "Comment.TextHorizontalAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun metin yatay hizalama türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/comment/texthorizontalalignment/
---
## Comment.TextHorizontalAlignment property

Yorumun metin yatay hizalama tipini alır ve ayarlar.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // İlk yatay hizalamayı Fill olarak ayarla
            comment.TextHorizontalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Initial alignment: " + comment.TextHorizontalAlignment);

            // Hizalamayı Center olarak değiştir, eğer Fill ise
            if (comment.TextHorizontalAlignment == TextAlignmentType.Fill)
            {
                comment.TextHorizontalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Updated alignment: " + comment.TextHorizontalAlignment);
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


