---
title: "CommentShape.Comment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CommentShape özelliği. Yorum nesnesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/commentshape/comment/
---
## CommentShape.Comment property

Yorum nesnesini alır.

```csharp
public Comment Comment { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentShapePropertyCommentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            
            // Yorum şekli alın ve Comment özelliğini gösterin
            CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
            Comment retrievedComment = commentShape.Comment;
            
            // Yorum metnini görüntüleyin
            Console.WriteLine("Comment Text: " + retrievedComment.Note);
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


