---
title: "Outline.SummaryColumnRight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Outline özelliği. Özet sütununun, ana hatta detay sütunlarının sağında konumlandırılıp konumlandırılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Anahattaki özet sütununun detay sütunlarının sağında konumlandırılıp konumlandırılmayacağını gösterir.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryColumnRightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekle ve satırları grupla
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Satırları grupla (bir ana hat oluşturur)
            worksheet.Cells.GroupRows(0, 9, false);

            // Ana hat ayarlarını al
            Outline outline = worksheet.Outline;

            // SummaryColumnRight'ı true olarak ayarla (özet sütunları detay sütunlarının sağında görünecek)
            outline.SummaryColumnRight = true;
            Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);

            // Çalışma kitabını kaydedin
            workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


