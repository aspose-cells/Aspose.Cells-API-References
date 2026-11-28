---
title: "PivotField.HideDetail"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Bir pivot alanındaki tüm PivotItem'ların detayının gizlenip gizlenmeyeceğini ayarlar. Bu, alanı daraltıp genişletir."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Bir pivot alanındaki tüm PivotItem'ların detayının gizlenip gizlenmeyeceğini ayarlar. Bu, alanı daraltıp genişletir.

```csharp
[Obsolete("Use PivotItemsCollection.HideAllDetails() and UnhideAllDetails() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideDetail(bool isHiddenDetail)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isHiddenDetail | Boolean | Pivot alanının detayını gizleyip gizlemeyeceği. |

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotItemsCollection.HideAllDetails() ve UnhideAllDetails() yöntemlerini kullanın. Bu yöntem, Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // İlk satır alanı için detayları gizle
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


