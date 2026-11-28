---
title: "AdvancedFilter.ListRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AdvancedFilter özelliği. Bu gelişmiş filtrenin liste aralığını alır"
type: docs
url: /tr/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

Bu gelişmiş filtrenin liste aralığını alır.

```csharp
public string ListRange { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek verileri doldur
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // Gelişmiş filtreyi kurun
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange yalnızca okunabilir ve filtre oluşturulurken otomatik olarak ayarlanır
            // Bunu yalnızca okuyabiliriz, doğrudan ayarlayamayız
            
            // Liste aralığını göster (otomatik olarak belirlenen aralığı gösterecek)
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // Çalışma kitabını kaydedin
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


