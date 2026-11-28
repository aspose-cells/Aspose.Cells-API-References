---
title: "ListObject.ShowTotals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Bu tablonun toplam satırını gösterip göstermediğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Bu TAble'ın toplam satırını gösterip göstermediğini alır ve ayarlar.

```csharp
public bool ShowTotals { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTotalsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluşturmak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(8);

            // Bir liste nesnesi/tablo oluştur
            int index = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject table = worksheet.ListObjects[index];

            // Toplam satırını etkinleştir ve bir hesaplama ayarla
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Çalışma kitabını kaydedin
            workbook.Save("ListObjectShowTotalsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


