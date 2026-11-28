---
title: "PivotTableCalculateOption.RefreshData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTableCalculateOption özelliği. Pivot tablonun veri kaynağının yenilenip yenilenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Pivot tablonun veri kaynağının yenilenip yenilenmeyeceğini gösterir.

```csharp
public bool RefreshData { get; set; }
```

### Açıklamalar

Doğru ise, veri kaynağından pivot önbelleğini yenileyin, ardından aynı pivot önbelleğine dayalı tüm pivot tabloları hesaplayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ayarla
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Kaynak veriyi değiştir
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // RefreshData seçeneğiyle pivot tabloyu hesapla
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // Güncellenmiş pivot tablo değerini çıktı olarak ver
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


