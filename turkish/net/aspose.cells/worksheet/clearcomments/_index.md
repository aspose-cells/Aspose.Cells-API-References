---
title: "Worksheet.ClearComments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Tasarımcı elektronik tablosundaki tüm yorumları temizler"
type: docs
url: /tr/net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

Tasarımcı elektronik tablosundaki tüm yorumları temizler.

```csharp
public void ClearComments()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücre referanslarını kullanarak hücrelere örnek yorumlar ekle
            int comment1 = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1].Note = "This is comment 1";
            
            int comment2 = worksheet.Comments.Add("B3");
            worksheet.Comments[comment2].Note = "This is comment 2";
            
            int comment3 = worksheet.Comments.Add("C5");
            worksheet.Comments[comment3].Note = "This is comment 3";

            // Temizlemeden önce yorum sayısını göster
            Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");

            // Çalışma sayfasındaki tüm yorumları temizle
            worksheet.ClearComments();

            // Temizledikten sonra yorum sayısını göster
            Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");

            // Çalışma kitabını kaydedin
            workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


