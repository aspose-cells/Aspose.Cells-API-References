---
title: "Worksheet.FirstVisibleColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. İlk görünen sütun indeksini temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

İlk görünen sütun indeksini temsil eder.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk sütunu gizle (indeks 0)
            worksheet.Cells.HideColumn(0);
            
            // İlk görünen sütun indeksini al ve göster
            Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FirstVisibleColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


