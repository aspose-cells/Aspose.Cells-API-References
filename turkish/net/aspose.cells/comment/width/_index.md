---
title: "Comment.Width"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun genişliğini piksel biriminde temsil eder."
type: docs
url: /tr/net/aspose.cells/comment/width/
---
## Comment.Width property

Yorumun genişliğini piksel biriminde temsil eder.

```csharp
public int Width { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Yorum özelliklerini ayarla
            comment.Note = "This is a sample comment";
            comment.Width = 200; // Setting the width of the comment box
            comment.Height = 50;
            
            // Çalışma kitabını kaydedin
            workbook.Save("CommentWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


