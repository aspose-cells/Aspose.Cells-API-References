---
title: "Comment.TextVerticalAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun metin dikey hizalama türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/comment/textverticalalignment/
---
## Comment.TextVerticalAlignment property

Yorumun metin dikey hizalama tipini alır ve ayarlar.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("B3");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Dikey hizalamayı Fill olarak ayarla
            comment.TextVerticalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);

            // Dikey hizalamayı Center olarak değiştir, eğer Fill ise
            if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
            {
                comment.TextVerticalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
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


