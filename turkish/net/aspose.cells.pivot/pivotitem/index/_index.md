---
title: "PivotItem.Index"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotItem özelliği. Önbellek alanındaki pivot öğesinin dizinini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotitem/index/
---
## PivotItem.Index property

Pivot öğesinin önbellek alanındaki dizinini alır.

```csharp
[Obsolete("Use PivotItem.Position property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Index { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotItem.Position özelliğini kullanın. Bu yöntem, Ağustos 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Satır alanını al
            PivotField rowField = pivotTable.RowFields[0];
            
            // Pivot öğelerine Index özelliğiyle erişin
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Item: {item.Value}, Index: {item.Index}");
                
                // Öğe detayını Index özelliğiyle gizle
                if (item.Value.ToString() == "Apple")
                {
                    rowField.HideItemDetail(item.Index, true);
                }
            }
            
            // Pivot tabloyu hesapla ve yenile
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotItemPropertyIndexDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


