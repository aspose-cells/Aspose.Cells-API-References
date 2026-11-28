---
title: "PivotFilter.GetTop10Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFilter yöntemi. Filtrenin ilk 10 ayarını alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfilter/gettop10value/
---
## PivotFilter.GetTop10Value method

Filtre için ilk 10 ayarını alır.

```csharp
public Top10Filter GetTop10Value()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetTop10ValueDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // İlk çalışma sayfasına ve pivot tabloya erişin
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // İlk temel alana ilk 10 filtresini uygula (sayısına göre ilk 2 öğeyi göster)
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Uygulanan filtreyi ve onun ilk 10 değerini al
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            Top10Filter top10Filter = filter.GetTop10Value();
            
            // Filtre ayrıntılarını çıktı olarak ver
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Top 10 Items: " + top10Filter.Items);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Top10Filter](../../../aspose.cells/top10filter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


