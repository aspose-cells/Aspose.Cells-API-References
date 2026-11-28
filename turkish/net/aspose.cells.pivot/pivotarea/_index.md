---
title: "Class PivotArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotArea sınıfı. Pivot tablonun seçilen alanını sunar"
type: docs
url: /tr/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

Pivot table'ın seçili alanını gösterir.

```csharp
public class PivotArea
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | PivotTable'ın seçilen alanını sunar. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | Bu kuralın uygulandığı PivotTable bölgesini alır ve ayarlar. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | Bu PivotArea için tüm filtreleri alır. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | Sütun toplamının dahil olup olmadığını gösterir. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | Kuralın, taslak modunda olan bir alana başvurup başvurmadığını gösterir. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | Satır toplamının dahil edilip edilmediğini gösterir. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | Bir öğe seçimi için yalnızca veri değerlerinin (görünümün veri alanında) seçilip seçilmediğini ve öğe etiketlerinin dahil edilmediğini gösterir. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | Bir öğe seçimi için yalnızca veri etiketlerinin seçilip seçilmediğini gösterir. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | Seçim kuralının türünü alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | Bu pivot alanının hücre alanlarını alır. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | Filtrelerle alanı seç. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | Bölgede bir alanı alan olarak seç. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | Bölgede bir alanı alan olarak seç. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Çalışma sayfasına bir pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Bir PivotArea örneği oluştur
            PivotArea pivotArea = new PivotArea(pivotTable);

            // PivotArea'nın özelliklerini ayarla
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // Belirli bir alanı seçmek için Select metodunu kullan
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


