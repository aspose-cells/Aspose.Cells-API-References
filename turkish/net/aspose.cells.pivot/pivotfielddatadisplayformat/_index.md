---
title: "Enum PivotFieldDataDisplayFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotFieldDataDisplayFormat enum. PivotTable veri alanındaki veri görüntüleme biçimini temsil eder."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfielddatadisplayformat/
---
## PivotFieldDataDisplayFormat enumeration

PivotTable veri alanındaki veri görüntüleme biçimini temsil eder.

```csharp
public enum PivotFieldDataDisplayFormat
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Normal | `0` | Normal görüntüleme biçimini temsil eder. |
| DifferenceFrom | `1` | Görüntüleme biçiminden farkı temsil eder. |
| PercentageOf | `2` | Görüntüleme biçiminin yüzdesini temsil eder. |
| PercentageDifferenceFrom | `3` | Görüntüleme biçiminden yüzde farkı temsil eder. |
| RunningTotalIn | `4` | Görüntüleme biçimindeki çalışan toplamı temsil eder. |
| PercentageOfRow | `5` | Satır görüntüleme biçiminin yüzdesini temsil eder. |
| PercentageOfColumn | `6` | Sütun görüntüleme biçiminin yüzdesini temsil eder. |
| PercentageOfTotal | `7` | Toplam görüntüleme biçiminin yüzdesini temsil eder. |
| Index | `8` | Dizin görüntüleme biçimini temsil eder. |
| PercentageOfParentRowTotal | `9` | Ebeveyn satır toplamının yüzde görüntüleme biçimini temsil eder. |
| PercentageOfParentColumnTotal | `10` | Ebeveyn sütun toplamının yüzde görüntüleme biçimini temsil eder. |
| PercentageOfParentTotal | `11` | Ebeveyn toplamının yüzde görüntüleme biçimini temsil eder. |
| PercentageOfRunningTotalIn | `12` | Görüntüleme biçimindeki çalışan toplamın yüzde değerini temsil eder. |
| RankSmallestToLargest | `13` | En küçükten en büyüğe görüntü formatını temsil eder. |
| RankLargestToSmallest | `14` | En büyükten en küçüğe görüntü formatını temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDataDisplayFormatDemo
    {
        public static void PivotFieldDataDisplayFormatExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Örnek veri ekleyin
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Bir pivot tablo ekle
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Pivot tablo stilini ayarla
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // PivotField'ın özniteliklerini değiştirin
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = "custom display name";

            // DataDisplayFormat'ı ayarla
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // Verileri yenile ve hesapla
            pivot.RefreshData();
            pivot.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


