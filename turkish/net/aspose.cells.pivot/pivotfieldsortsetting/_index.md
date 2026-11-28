---
title: "Class PivotFieldSortSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting sınıfı. Pivot alanlarını sıralama ayarını temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

Pivot alanlarını sıralama ayarını temsil eder.

```csharp
public class PivotFieldSortSetting
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | Satır veya sütuna göre değerleri sıralar. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**Obsolete.**) Sıralanan alanın dizinini temsil eder. -1, PivotField'i etiketlere göre sıraladığı anlamına gelir, diğerleri veri alanına göre sıralama anlamına gelir. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | Basit bir veri sıralama işleminin uygulanıp uygulanmayacağını gösterir. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | Alanı kendi içinde mi yoksa veri alanına göre mi sıralayacağını gösterir. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | Pivot satır türü sıralama ölçütü. |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | Sıralama yapılan alanın dizinini temsil eder. -1 değeri, pivot öğesinin kendi değerlerine göre sıralama yapıldığını gösterir. Sıfır veya daha büyük olduğunda, veri bölgesindeki veri alanının dizinini temsil eder. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | [`SortOrder`](../../aspose.cells/sortorder/) temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot tablodan pivot alanı sıralama ayarını al
            // Not: Bu, pivot tablonun erişebileceğimiz sıralama ayarlarına sahip olduğunu varsayar
            // Yeni bir PivotFieldSortSetting doğrudan oluşturamadığımız için
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // Görüntüleme özellikleri (yalnızca okunur)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // Pivot tabloya sıralamayı uygula (gerçek sıralama, pivot tablo yöntemleriyle yapılır)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Sonucu kaydet
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


