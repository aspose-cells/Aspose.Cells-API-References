---
title: "Comment.HeightCM"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment özelliği. Yorumun santimetre birimindeki yüksekliğini temsil eder"
type: docs
url: /tr/net/aspose.cells/comment/heightcm/
---
## Comment.HeightCM property

Yorumun yüksekliğini santimetre biriminde temsil eder.

```csharp
public double HeightCM { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightCMDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Yorum metnini ayarla
            comment.Note = "Sample comment";
            
            // Yorum yüksekliğini santimetre cinsinden ayarla
            comment.HeightCM = 1.5;
            
            // Çalışma kitabını kaydedin
            workbook.Save("CommentHeightCMDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


