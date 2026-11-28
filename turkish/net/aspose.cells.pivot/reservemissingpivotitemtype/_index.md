---
title: "Enum ReserveMissingPivotItemType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.ReserveMissingPivotItemType enum. Eksik pivot öğelerinin nasıl tutulacağını temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/reservemissingpivotitemtype/
---
## ReserveMissingPivotItemType enumeration

Eksik pivot öğelerinin nasıl tutulacağını temsil eder.

```csharp
public enum ReserveMissingPivotItemType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | Eski eksik pivot öğelerini kaldırır ve yeni veri kaynağının silinen öğelerini eksik öğeler olarak tutar. |
| All | `1` | Tüm eksik öğeleri tutar. |
| None | `2` | Tüm eksik pivot öğelerini kaldırır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class ReserveMissingPivotItemTypeDemo
    {
        public static void ReserveMissingPivotItemTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir PivotTable ekle
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // PivotTable'a alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // ReserveMissingPivotItemType seçeneğini ayarla
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Belirtilen seçeneklerle PivotTable'ı hesapla
            pivotTable.CalculateData(calculateOption);

            // PivotTable'ı yenile
            pivotTable.RefreshData();

            // Çalışma kitabını kaydedin
            workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


