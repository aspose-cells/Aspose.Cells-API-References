---
title: "PivotField.HideItemDetail"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Bir pivot alanındaki belirli PivotItem'ın gizli detay olup olmadığını ayarlar"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

Belirli bir pivot alanındaki PivotItem'ın gizli detay olup olmadığını ayarlar.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItemDetail(int index, bool isHiddenDetail)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | pivotField içindeki pivotItem'ın indeksi. |
| isHiddenDetail | Boolean | belirli PivotItem'ın gizli olup olmadığı |

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.PivotItems[int].IsDetailHidden özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 12 ay içinde kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemDetailWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("SampleData.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Pivot tablo ekle
            int index = worksheet.PivotTables.Add("A1:B5", "H5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Alanları bölgelere ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];
            
            // İndeks 2'deki (East) öğe detayını isHidden=false ile gizle
            pivotField.HideItemDetail(2, false);
            
            // Pivot tablo verilerini yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTable_HideItemDetail_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


