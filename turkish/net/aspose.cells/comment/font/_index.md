---
title: "Comment.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun yazı tipini alır"
type: docs
url: /tr/net/aspose.cells/comment/font/
---
## Comment.Font property

Yorumun yazı tipini alır.

```csharp
public Font Font { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";

            // Yorumun yazı tipi özelliklerine eriş ve değiştir
            Aspose.Cells.Font font = comment.Font;
            font.Size = 12;
            font.Name = "Arial";
            font.Color = System.Drawing.Color.Red;
            font.IsBold = true;

            // Çalışma kitabını kaydedin
            workbook.Save("CommentFontDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


