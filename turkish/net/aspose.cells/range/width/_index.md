---
title: "Range.Width"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Bir aralığın genişliğini puan cinsinden alır"
type: docs
url: /tr/net/aspose.cells/range/width/
---
## Range.Width property

Bir aralığın genişliğini nokta cinsinden alır.

```csharp
public double Width { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Width özelliğini göstermek için sütun genişliklerini ayarla
            worksheet.Cells.SetColumnWidth(1, 20); // Column B width = 20
            worksheet.Cells.SetColumnWidth(2, 30); // Column C width = 30
            
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Aralık genişliğini göster (aralıktaki sütun genişliklerinin toplamı)
            Console.WriteLine("Range Width: " + range.Width);
            
            // Doğrulama için bireysel özellikleri göster
            Console.WriteLine("Range Left Position: " + range.Left);
            Console.WriteLine("Range Top Position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


