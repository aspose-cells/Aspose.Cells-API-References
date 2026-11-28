---
title: "SubtotalSetting.TotalList"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SubtotalSetting özelliği. Alt toplamların ekleneceği alanları gösteren sıfır tabanlı alan offsetlerinden oluşan bir dizi"
type: docs
url: /tr/net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

Alt toplamların eklendiği alanları gösteren, sıfır tabanlı alan ofsetlerinden oluşan bir dizi.

```csharp
public int[] TotalList { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyTotalListDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri kurulumu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Alt toplamı oluştur ve uygula
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);

            // TotalList kullanımını göstermek için alt toplam ayarını al
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
            
            // Çalışma kitabını kaydedin
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


