---
title: "AutoFilter.Range"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter özelliği. Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder"
type: docs
url: /tr/net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder.

```csharp
public string Range { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["A5"].PutValue("Item4");

            // A1:A5 aralığına otomatik filtre uygula
            sheet.AutoFilter.Range = "A1:A5";

            // Otomatik filtre aralığını göster
            Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFilterRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


