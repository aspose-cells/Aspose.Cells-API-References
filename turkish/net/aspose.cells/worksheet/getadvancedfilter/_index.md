---
title: "Worksheet.GetAdvancedFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Gelişmiş filtrenin ayarlarını alır"
type: docs
url: /tr/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

Gelişmiş filtrenin ayarlarını alır.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Filtreleme için verileri ayarla
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // Kriter aralığını ayarla
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // Gelişmiş filtreyi uygula
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // Gelişmiş filtreyi al
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // Filtre aralıklarını çıktı olarak ver
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### Ayrıca Bakınız

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


