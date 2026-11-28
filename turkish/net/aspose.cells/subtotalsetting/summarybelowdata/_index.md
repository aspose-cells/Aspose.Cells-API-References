---
title: "SubtotalSetting.SummaryBelowData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SubtotalSetting özelliği. Verinin altında özet eklenip eklenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/subtotalsetting/summarybelowdata/
---
## SubtotalSetting.SummaryBelowData property

Verilerin altında özet eklenip eklenmeyeceğini gösterir.

```csharp
public bool SummaryBelowData { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySummaryBelowDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Alt toplamlar için hücre alanı oluştur
            CellArea area = CellArea.CreateCellArea("A1", "B5");

            // Gerekli tüm parametrelerle Cells.Subtotal yöntemini kullanarak alt toplamları uygula
            worksheet.Cells.Subtotal(
                area, 
                0, 
                ConsolidationFunction.Sum, 
                new int[] { 1 }, 
                false, 
                false, 
                false);  // summaryBelowData parameter

            // SummaryBelowData özelliğini kontrol etmek için ayarı alın
            SubtotalSetting retrievedSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // SummaryBelowData özelliği değerini çıktı olarak ver
            Console.WriteLine("SummaryBelowData: " + retrievedSetting.SummaryBelowData);
        }
    }
}
```

### Ayrıca Bakınız

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


