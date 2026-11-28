---
title: "Comment.TextOrientationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun metin yönlendirme tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/comment/textorientationtype/
---
## Comment.TextOrientationType property

Yorumun metin yönlendirme tipini alır ve ayarlar.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // İlk yönlendirmeyi NoRotation olarak ayarlayın
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Initial orientation: " + comment.TextOrientationType);

            // Yönlendirmeyi TopToBottom olarak değiştir, eğer şu anda NoRotation ise
            if (comment.TextOrientationType == TextOrientationType.NoRotation)
            {
                comment.TextOrientationType = TextOrientationType.TopToBottom;
                Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CommentOrientationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


