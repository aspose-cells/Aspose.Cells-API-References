---
title: "PivotTable.ShowReportFilterPageByIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. PageFields içindeki konum indeksine göre tüm rapor filtre sayfalarını göster"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

PageFields içindeki konum indeksine göre tüm rapor filtre sayfalarını göster.

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| posIndex | Int32 | PageFields içindeki konum indeksi |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("PivotTable.xlsx");
            
            // Pivot tabloyu içeren ilk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Sayfa alanının indeksine (konumuna) göre rapor filtre sayfalarını göster
            int pageFieldIndex = 0; // First page field
            pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


