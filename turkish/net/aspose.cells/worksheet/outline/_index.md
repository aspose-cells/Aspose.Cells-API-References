---
title: "Worksheet.Outline"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bu çalışma sayfasındaki taslağı alır"
type: docs
url: /tr/net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Bu çalışma sayfasındaki anahattı alır.

```csharp
public Outline Outline { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOutlineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin ve taslak grupları oluşturun
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
                worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
            }

            // Satırları gruplayın (taslak oluşturur)
            worksheet.Cells.GroupRows(0, 9, false);

            // Taslak özelliklerine erişin
            Outline outline = worksheet.Outline;
            Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
            Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");

            // Taslak ayarlarını değiştirin
            outline.SummaryRowBelow = true;
            outline.SummaryColumnRight = false;

            // Taslak işlevselliğini göstermek için satırları gruptan çıkarın
            worksheet.Cells.UngroupRows(0, 9);

            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetOutlineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


