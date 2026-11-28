---
title: "Sınıf PivotTableCalculateOption"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotTableCalculateOption sınıfı. Pivot tablo verilerini hesaplama seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

Pivot tablo verilerini hesaplama seçeneklerini temsil eder.

```csharp
public class PivotTableCalculateOption
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | Bu pivot tabloya dayalı olarak grafiklerin yenilenip yenilenmeyeceğini gösterir. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | Pivot tablonun veri kaynağının yenilenip yenilenmeyeceğini gösterir. |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | Veri kaynağının pivot önbelleğine yenilenmesi için seçenekleri alır ve ayarlar. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | Eksik pivot öğelerinin nasıl saklanacağını temsil eder. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Pivot tablo için bazı veriler ekleyin.
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Çalışma sayfasına bir pivot tablo ekle
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Bir PivotTableCalculateOption nesnesi oluştur
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Belirtilen seçeneklerle pivot tablo verilerini hesapla
            pivotTable.CalculateData(calculateOption);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


