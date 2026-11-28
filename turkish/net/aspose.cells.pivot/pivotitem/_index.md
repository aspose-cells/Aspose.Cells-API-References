---
title: "Sınıf PivotItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotItem sınıfı. PivotField raporunda bir öğeyi temsil eder."
type: docs
url: /tr/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

PivotField raporundaki bir öğeyi temsil eder.

```csharp
public class PivotItem
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | (**Obsolete.**) Pivot öğesinin önbellek alanındaki dizinini alır. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | Bu pivot öğesinin hesaplanmış bir formül öğesi olup olmadığını gösterir. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | Bu pivot öğesinin detayının gizli olup olmadığını alır ve ayarlar. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsolete.**) Bu pivot öğesinin hesaplanmış bir formül öğesi olup olmadığını gösterir. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Pivot öğesinin gizli olup olmadığını alır ve ayarlar. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsolete.**) Pivot öğesinin detayı gizleyip gizlemediğini alır ve ayarlar. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Öğenin veri kaynağından kaldırılıp kaldırılmadığını gösterir. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | Pivot öğesinin adını alır. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Bu öğenin alandaki tüm PivotItems içinde dizinini belirtir. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | (**Obsolete.**) Aynı üst düğüm altındaki PivotItems içinde konum dizinini belirtir. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Pivot öğesinin değerini alır |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Pivot öğesinin tarih saat değerini alır. Değer null ise DateTime.MinValue döndürülür. |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Pivot öğesinin çift değerini alır. Değer null veya sayı değilse, 0 döndürür. |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Bu hesaplanmış öğenin formülünü alır. Yalnızca öğe hesaplanmış bir öğe olduğunda çalışır. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Pivot öğesinin metin değerini alır. Değer null ise, "" döndürür. |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move)(int) | Öğeyi pivot alanında yukarı ya da aşağı hareket ettirir |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move_1)(int, bool) | (**Obsolete.**) Öğeyi yukarı ya da aşağı hareket ettirir |

## Alanlar

| Ad | Açıklama |
| --- | --- |
| const [AllPageItemsIndex](../../aspose.cells.pivot/pivotitem/allpageitemsindex/) | Sayfa öğelerinin tümünü seçme belirteci dizini (0x7FFD, geçerli bir dizin değil) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemDemo
    {
        public static void PivotItemExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Çalışma sayfasına bir pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Pivot öğelere erişin
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Pivot öğesinin adını yazdır
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // Özellikleri ayarla
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Pivot öğesinin değerini yazdır
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // Yöntemleri kullan
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PivotItemExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


