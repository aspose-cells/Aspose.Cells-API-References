---
title: "MsoFillFormat.Transparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormat özelliği. Belirtilen doldurmanın şeffaflık derecesini 0.0 opak'tan 1.0 tamamen şeffaf'a kadar bir değer olarak döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Belirtilen dolgunun şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar.

```csharp
public double Transparency { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyTransparencyDemo
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

            // Şeffaflık dahil dolgu biçim özelliklerini ayarla
            comment.CommentShape.FillFormat.IsVisible = true;
            comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
            comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
            
            // Şeffaflığı ayarla (0.0 = tamamen opak, 1.0 = tamamen şeffaf)
            comment.CommentShape.FillFormat.Transparency = 0.5;

            // Çalışma kitabını kaydedin
            workbook.Save("CommentTransparencyDemo.xlsx");

            // Şeffaflığı doğrulamak için kaydedilmiş çalışma kitabını yükle
            Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
            Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
            
            // Şeffaflık değerini çıktı olarak vererek kaydedildiğini ve doğru yüklendiğini göster
            Console.WriteLine("Comment fill transparency: " + 
                verifyComment.CommentShape.FillFormat.Transparency);
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


