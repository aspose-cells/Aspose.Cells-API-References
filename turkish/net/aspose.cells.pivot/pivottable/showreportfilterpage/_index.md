---
title: "PivotTable.ShowReportFilterPage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. PivotField'e göre tüm rapor filtre sayfalarını göster; PivotField, PageFields içinde bulunmalıdır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

PivotField'e göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageField | PivotField | PivotField nesnesi |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("source.xlsx");
            
            // İlk çalışma sayfasına ve pivot tabloya erişin
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Her sayfa alanı için rapor filtre sayfalarını göster
            foreach (PivotField pageField in pivotTable.PageFields)
            {
                pivotTable.ShowReportFilterPage(pageField);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


