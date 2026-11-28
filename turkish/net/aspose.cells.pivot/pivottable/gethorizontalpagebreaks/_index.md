---
title: "PivotTable.GetHorizontalPageBreaks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Bu pivot tablonun yatay sayfa sonlarını alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/gethorizontalpagebreaks/
---
## PivotTable.GetHorizontalPageBreaks method

Bu pivot tablonun yatay sayfa sonlarını alır.

```csharp
public int[] GetHorizontalPageBreaks()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetHorizontalPageBreaksDemo
    {
        public static void Run()
        {
            // Kaynak dosyadan bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("pivot_pagebreaks.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Pivot tablo verilerini yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Yatay sayfa sonlarını al
            int[] pageBreaks = pivotTable.GetHorizontalPageBreaks();
            
            // Sonuçları görüntüleyin
            Console.WriteLine("Horizontal Page Breaks:");
            foreach (int row in pageBreaks)
            {
                Console.WriteLine("Row: " + row);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


