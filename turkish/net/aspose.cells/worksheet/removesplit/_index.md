---
title: "Worksheet.RemoveSplit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bölünmüş pencereyi kaldırır"
type: docs
url: /tr/net/aspose.cells/worksheet/removesplit/
---
## Worksheet.RemoveSplit method

Bölünmüş pencereyi kaldırır.

```csharp
public void RemoveSplit()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveSplitDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını böl
            worksheet.Split();
            Console.WriteLine("Worksheet split state: " + worksheet.PaneState);
            
            // Bölmeyi kaldır
            worksheet.RemoveSplit();
            Console.WriteLine("Worksheet split state after RemoveSplit: " + worksheet.PaneState);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


