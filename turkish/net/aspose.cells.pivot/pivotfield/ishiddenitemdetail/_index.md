---
title: "PivotField.IsHiddenItemDetail"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Belirli PivotItem'ın ayrıntısını gizleyip gizlemeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

Belirli PivotItem'ın ayrıntısını gizleyip gizlemeyeceğini gösterir..

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItemDetail(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | pivotField içindeki pivotItem'ın dizini. |

### Dönüş Değeri

belirli PivotItem'ın ayrıntısının gizli olup olmadığı

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.PivotItems[int].IsDetailHidden özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 12 ay içinde kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemDetailWithInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Country";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Japan";
            cells["A3"].Value = "Japan";
            cells["A4"].Value = "USA";
            cells["A5"].Value = "USA";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;
            cells["B5"].Value = 4000;

            // Pivot tablo ekle
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];
            
            // İndeks 1 (ABD) için öğe ayrıntısını gizle
            pivotField.HideItemDetail(1, true);
            
            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Öğe ayrıntısının gizli olup olmadığını kontrol et
            Console.WriteLine("Is item at index 1 hidden? " + pivotField.IsHiddenItemDetail(1));
            
            // Çalışma kitabını kaydet
            workbook.Save("PivotFieldIsHiddenItemDetailDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


