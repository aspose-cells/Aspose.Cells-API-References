---
title: "Range.Left"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. A sütununun sol kenarından aralığın sol kenarına kadar olan mesafeyi puan cinsinden alır."
type: docs
url: /tr/net/aspose.cells/range/left/
---
## Range.Left property

A sütununun sol kenarından aralığın sol kenarına kadar olan mesafeyi, nokta cinsinden alır.

```csharp
public double Left { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B2'den C4'e bir aralık oluştur
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Left özelliğinin kullanımını göster
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
            
            // Test durumuna göre beklenen değerleri hesapla
            double expectedLeft = 64 / 96.0 * 72;
            Console.WriteLine("Expected Left position: " + expectedLeft);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


