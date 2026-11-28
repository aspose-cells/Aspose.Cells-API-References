---
title: "Comment.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/comment/row/
---
## Comment.Row property

Yorumun satır indeksini alır.

```csharp
public int Row { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyRowDemo
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

            // Yorum yapılan hücrenin satır indeksini al ve göster
            int row = comment1.Row;
            Console.WriteLine("The comment is in row: " + row);

            // B3 hücresine başka bir yorum ekle
            commentIndex = worksheet.Comments.Add("B3");
            Comment comment2 = worksheet.Comments[commentIndex];
            comment2.Note = "Another comment";

            // İkinci yorumun satır indeksini göster
            Console.WriteLine("Second comment is in row: " + comment2.Row);
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


