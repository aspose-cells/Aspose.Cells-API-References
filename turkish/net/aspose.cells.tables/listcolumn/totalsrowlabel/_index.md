---
title: "ListColumn.TotalsRowLabel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListColumn özelliği. Toplam satırının görüntüleme etiketlerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listcolumn/totalsrowlabel/
---
## ListColumn.TotalsRowLabel property

Toplam satırının görüntüleme etiketlerini alır ve ayarlar.

```csharp
public string TotalsRowLabel { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyTotalsRowLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(200);

            // Tablo oluşturun
            int index = worksheet.ListObjects.Add(0, 0, 4, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Toplam satırını yapılandır
            ListColumn priceColumn = table.ListColumns[1];
            priceColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            priceColumn.TotalsRowLabel = "Grand Total";

            workbook.Save("ListColumnTotalsRowLabelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


