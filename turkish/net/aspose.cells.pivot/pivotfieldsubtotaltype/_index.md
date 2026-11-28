---
title: "Enum PivotFieldSubtotalType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotFieldSubtotalType enum. PivotFieldSubtotalType için özet açıklama"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

PivotFieldSubtotalType için özet açıklama.

```csharp
[Flags]
public enum PivotFieldSubtotalType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Hiçbiri alt toplam türünü temsil eder. |
| Automatic | `1` | Otomatik alt toplam türünü temsil eder. |
| Sum | `2` | Toplam alt toplam türünü temsil eder. |
| Count | `4` | Sayı alt toplam türünü temsil eder. |
| Average | `8` | Ortalama alt toplam türünü temsil eder. |
| Max | `10` | Maksimum alt toplam türünü temsil eder. |
| Min | `20` | Minimum alt toplam türünü temsil eder. |
| Product | `40` | Çarpım alt toplam türünü temsil eder. |
| CountNums | `80` | Count Nums alt toplam türünü temsil eder. |
| Stdev | `100` | Standart Sapma alt toplam türünü temsil eder. |
| Stdevp | `200` | Popülasyonun Standart Sapması alt toplam türünü temsil eder. |
| Var | `400` | Varyans alt toplam türünü temsil eder. |
| Varp | `800` | Popülasyonun Varyansı alt toplam türünü temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Bir pivot tablo ekle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Satır alanı için alt toplam türünü ayarla
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // Özet tablo verilerini yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


