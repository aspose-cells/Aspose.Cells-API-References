---
title: "Comment.IsVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun görünür olup olmadığını temsil eder"
type: docs
url: /tr/net/aspose.cells/comment/isvisible/
---
## Comment.IsVisible property

Yorumun görünür olup olmadığını temsil eder.

```csharp
public bool IsVisible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Yorumu görünür yap
            comment.IsVisible = true;

            // Yorumun görünür olup olmadığını kontrol et
            if (comment.IsVisible)
            {
                Console.WriteLine("The comment is visible");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CommentVisibilityDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


