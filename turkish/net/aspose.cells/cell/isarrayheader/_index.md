---
title: "Cell.IsArrayHeader"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrenin formülünün bir dizi formülü olduğunu ve dizinin ilk hücresi olduğunu gösterir"
type: docs
url: /tr/net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

Hücrenin formülünün bir dizi formülü olduğunu ve dizinin ilk hücresi olduğunu gösterir.

```csharp
public bool IsArrayHeader { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayHeaderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B2:D4 aralığında bir dizi formülü oluştur
            worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
            
            // IsArrayHeader özelliğini doğrula ve yazdır
            // Not: IsArrayHeader yalnızca okunabilir ve dizi formülü başlıkları için otomatik olarak ayarlanır
            Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
            Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


