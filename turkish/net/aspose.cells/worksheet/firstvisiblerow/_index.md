---
title: "Worksheet.FirstVisibleRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. İlk görünen satır indeksini temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

İlk görünen satır indeksini temsil eder.

```csharp
public int FirstVisibleRow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı örnek veri ayarlayın
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // İlk görünen satırı 20. satıra ayarla
            worksheet.FirstVisibleRow = 20;
            
            // İlk görünen satırı göster
            Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FirstVisibleRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


