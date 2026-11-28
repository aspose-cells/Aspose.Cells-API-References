---
title: "Enum PivotItemPositionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotItemPositionType enum. ShowDataAs hesaplaması kullanıldığında temel alandaki pivot temel öğesinin konum türünü temsil eder."
type: docs
url: /tr/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

ShowDataAs hesabı kullanıldığında temel alandaki pivot temel öğesinin konum türünü temsil eder.

```csharp
public enum PivotItemPositionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Previous | `0` | PivotField içinde önceki pivot öğesini temsil eder. |
| Next | `1` | PivotField içinde sonraki pivot öğesini temsil eder. |
| Custom | `2` | PivotField içindeki pivot öğesinin indeksine göre farklı formatta değerleri gösterir. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
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

            // Çalışma sayfasına bir pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // Veri görüntüleme formatını, değerleri önceki öğeden fark olarak gösterecek şekilde ayarlayın
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // Pivot tabloyu yenileyin ve hesaplayın
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


