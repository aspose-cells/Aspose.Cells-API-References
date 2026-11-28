---
title: "MsoLineFormat.Weight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormat özelliği. Çizginin ağırlığını pt biriminde döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Çizginin kalınlığını puan (pt) biriminde döndürür veya ayarlar.

```csharp
public double Weight { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyWeightDemo
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
            
            // Yorum şeklinin satır biçimine eriş ve ağırlığı ayarla
            comment.CommentShape.LineFormat.Weight = 0.75;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Ağırlığın doğru ayarlandığını doğrula
            Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


