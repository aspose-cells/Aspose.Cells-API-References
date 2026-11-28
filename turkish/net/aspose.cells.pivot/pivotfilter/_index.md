---
title: "Sınıf PivotFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotFilter class. PivotFilter Koleksiyonunda bir PivotFilter'ı temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

PivotFilter Koleksiyonu içinde bir PivotFilter'ı temsil eder.

```csharp
public class PivotFilter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Obsolete.**) Pivot filtresinin otomatik filtresini alır. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | Pivot filtresinin Değerlendirme Sırasını alır. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | Bu pivot filtrenin uygulandığı kaynak alanın dizinini alır. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | Bu filtrenin kategorisini alır. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | Pivot filtresinin filtre tipini alır. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | Ölçü küp alanının dizinini belirtir. Bu özellik yalnızca OLAP pivotlarındaki filtreler tarafından kullanılır ve bir değer filtresinin hangi ölçüye uygulanacağını belirtir. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Obsolete.**) Pivot filtresinin ölçü alanı dizinini alır. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | Pivot filtresinin üye özellik alanı dizinini alır. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | Pivot filtresinin adını alır. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | Tarih filtreleme ölçütlerinde tam gün kullanılıp kullanılmayacağını gösterir. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | Etiket pivot filtresinin string değer1'ini alır. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | Etiket pivot filtresinin string değer2'sini alır. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | Değer bölgesindeki değer alanının dizinini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | Numara filtresinin değerlerini alır. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | Başlık filtresinin etiketlerini alır. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | Numara filtresinin değerlerini alır. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | Filtre için ilk 10 ayarını alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterDemo
    {
        public static void PivotFilterExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Çalışma sayfasını örnek verilerle doldur.
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

            // Çalışma sayfasına bir pivot tablo ekle
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Pivot tablo stilini ayarla
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Bir pivot filtresi ekle
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Pivot filtresi için ek özellikleri ayarla
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Özet tablo verilerini yenile ve hesapla
            pivot.RefreshData();
            pivot.CalculateData();

            // Çalışma kitabını kaydedin
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


