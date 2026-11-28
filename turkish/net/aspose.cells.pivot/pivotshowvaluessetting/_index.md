---
title: "Sınıf PivotShowValuesSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotShowValuesSetting sınıfı. ShowDataAs hesaplaması kullanıldığında değerlerin gösterilmesiyle ilgili ayarları temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

ShowDataAs hesabı kullanıldığında değerlerin nasıl gösterileceğiyle ilgili ayarları temsil eder.

```csharp
public class PivotShowValuesSetting
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | ShowDataAs hesaplaması kullanıldığında bir ShowDataAs hesaplaması için temel alanı temsil eder. |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | Pivot temel alanının başlığını alır. |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | Temel alandaki pivot öğesinin başlığını alır. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | ShowDataAs hesaplaması kullanıldığında temel alandaki pivot öğesinin özel indeksini temsil eder. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) ShowDataAs hesaplaması kullanıldığında temel alandaki temel pivot öğesinin türünü temsil eder. Çünkü PivotItemPosition.Custom yalnızca okuma içindir, PivotItemPosition.Custom ayarlamanız gerekiyorsa, lütfen PivotField.BaseItemIndex özniteliğini ayarlayın. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) Pivot raporunda bir veri alanının değerlerinin nasıl gösterileceğini temsil eder. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | Pivot raporunda bir veri alanının değerlerinin nasıl gösterileceğini alır ve ayarlar. |

## Alanlar

| Ad | Açıklama |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | Özel temel öğe indeksi: sonraki pivot öğesini kullan. "Show Values As" hesaplamaları için geçerlidir; Excel 2010 ve sonraki sürümlerde etkilidir. |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | Özel temel öğe indeksi: önceki pivot öğesini kullan. "Show Values As" hesaplamaları için geçerlidir; Excel 2010 ve sonraki sürümlerde etkilidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingDemo
    {
        public static void PivotShowValuesSettingExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // Çalışma sayfasına bir pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Veri alanına erişin
            PivotField dataField = pivotTable.DataFields[0];

            // ShowValuesSetting özelliğine erişin
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // PivotShowValuesSetting özelliklerini ayarlayın
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // Özet tablo verilerini yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


