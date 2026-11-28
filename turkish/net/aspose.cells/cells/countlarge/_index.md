---
title: "Cells.CountLarge"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Oluşturulan Cell nesnelerinin toplam sayısını alır"
type: docs
url: /tr/net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Oluşturulmuş Cell nesnelerinin toplam sayısını alır.

```csharp
public long CountLarge { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyCountLargeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B2"].PutValue("World");
            worksheet.Cells["C3"].PutValue(123);
            
            // CountLarge özelliğini göster
            long cellCount = worksheet.Cells.CountLarge;
            Console.WriteLine($"Total cells in worksheet: {cellCount}");
            
            // Demonstrasyon için kağıt boyutunu göster
            Console.WriteLine($"Paper Height: {worksheet.PageSetup.PaperHeight}");
            Console.WriteLine($"Paper Width: {worksheet.PageSetup.PaperWidth}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


