---
title: "Worksheet.PivotTables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bu çalışma sayfasındaki tüm özet tabloları alır"
type: docs
url: /tr/net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Bu çalışma sayfasındaki tüm pivot tabloları alır.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Örnekler

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPivotTablesDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasından özet tablo koleksiyonuna eriş
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Herhangi bir özet tablo olup olmadığını kontrol et
            if (pivotTables.Count > 0)
            {
                // İlk özet tabloyu al
                PivotTable pivotTable = pivotTables[0];
                
                // Mevcut filtreleri temizle
                pivotTable.PivotFilters.Clear();
                
                // Özet tablo verilerini yenile
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                
                // Değiştirilmiş çalışma kitabını kaydet
                workbook.Save("PivotTableModified.xlsx");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


