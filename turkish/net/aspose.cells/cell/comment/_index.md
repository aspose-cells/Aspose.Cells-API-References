---
title: "Cell.Comment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrenin yorumunu alır"
type: docs
url: /tr/net/aspose.cells/cell/comment/
---
## Cell.Comment property

Bu hücrenin yorumunu alır.

```csharp
public Comment Comment { get; }
```

### Açıklamalar

Hücreye uygulanacak yorum yoksa, null döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // Hücreye bir yorum ekle
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // Yorum yoksa yeni bir yorum oluştur
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // Yorum özelliklerini göster
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // Bazı yorum özelliklerini değiştir
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // Güncellenmiş yorum notunu göster
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // Çalışma kitabını kaydedin
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


