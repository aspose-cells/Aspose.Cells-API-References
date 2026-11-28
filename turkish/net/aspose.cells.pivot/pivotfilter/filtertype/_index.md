---
title: "PivotFilter.FilterType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFilter özelliği. Pivot filtrenin filtre tipini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfilter/filtertype/
---
## PivotFilter.FilterType property

Pivot filtresinin filtre tipini alır.

```csharp
public PivotFilterType FilterType { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // İlk çalışma sayfasına ve pivot tabloya erişin
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // İlk temel alana değer filtresi uygula (2'den küçük)
            pivotTable.BaseFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 2, 0);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Filtreyi doğrulamak için çalışma kitabını yeniden yükle
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            PivotTable verifyPivotTable = verifyWorkbook.Worksheets[0].PivotTables[0];
            
            // Uygulanan filtreyi al ve FilterType özelliğini göster
            PivotFilter filter = verifyPivotTable.BaseFields[0].GetFilters()[0];
            Console.WriteLine("Filter Type: " + filter.FilterType); // Should output ValueLessThan
            Console.WriteLine("Filter Value: " + filter.GetNumberValues()[0]); // Should output 2
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


