---
title: "Comment.AutoSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. Not: Mac ortamı gibi bazı özel durumlarda bu ayar etkili olmayabilir. Bu ayar etkili olmazsa lütfen FitToTextSize ile değiştirin."
type: docs
url: /tr/net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

Yorumun boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. Not: Bazı özel durumlarda (örneğin Mac ortamı) bu ayar etkili olmayabilir. Bu ayar etkili olmazsa, lütfen FitToTextSize() ile değiştirin.

```csharp
public bool AutoSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment that will auto-size to fit its content.";

            // AutoSize'ı true olarak ayarla
            comment.AutoSize = true;

            // Çalışma kitabını kaydedin
            workbook.Save("CommentAutoSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


