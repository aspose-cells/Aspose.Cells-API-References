---
title: "Sınıf PivotAreaFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotAreaFilter sınıfı. PivotTable için PivotArea filtresini temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

[`PivotArea`](../pivotarea/) için [`PivotTable`](../pivottable/) filtresini temsil eder.

```csharp
public class PivotAreaFilter
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | Bu filtrenin başvurduğu kaynak alanlardaki alanın dizinini alır. -2 değeri değerler alanını gösterir. |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | Bu alanın seçimi olup olmadığını gösterir. Yalnızca PivotTable Taslak görünümünde çalışır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | Bu filtre için hangi alt toplamın ayarlandığını alır. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | Filtre için alt toplam. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri kurulumu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // PivotTable oluştur - dönüş değeri işleme düzeltmesi
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // PivotAreaFilter oluştur ve yapılandır
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // Yöntemleri göster
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


