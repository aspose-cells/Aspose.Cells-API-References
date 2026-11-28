---
title: "Range.Top"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Satır 1'in üst kenarından aralığın üst kenarına olan mesafeyi puan cinsinden alır."
type: docs
url: /tr/net/aspose.cells/range/top/
---
## Range.Top property

1. satırın üst kenarından aralığın üst kenarına kadar olan mesafeyi, nokta cinsinden alır.

```csharp
public double Top { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyTopDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir aralık oluştur ve bazı değerler ayarla.
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            range[0, 0].PutValue("Test");
            
            // Top özelliğinin kullanımını göster.
            Console.WriteLine("Range Top position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


