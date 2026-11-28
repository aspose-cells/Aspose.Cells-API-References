---
title: "Comment.CommentShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Belirtilen yoruma ekli şekli temsil eden bir Shape nesnesi al."
type: docs
url: /tr/net/aspose.cells/comment/commentshape/
---
## Comment.CommentShape property

Belirtilen yoruma ekli şekli temsil eden bir Shape nesnesi al.

```csharp
public CommentShape CommentShape { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentPropertyCommentShapeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // CommentShape'i al ve özelliklerini değiştir
            Shape shape = comment1.CommentShape;
            shape.Width = 200;
            shape.Height = 100;
            shape.FillFormat.ForeColor = System.Drawing.Color.LightYellow;
            shape.LineFormat.ForeColor = System.Drawing.Color.Blue;

            // Şekil boyutlarını göster
            Console.WriteLine("Comment shape width: " + shape.Width);
            Console.WriteLine("Comment shape height: " + shape.Height);
        }
    }
}
```

### Ayrıca Bakınız

* class [CommentShape](../../../aspose.cells.drawing/commentshape/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


