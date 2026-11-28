---
title: "PivotTable.ShowDrill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Genişletme/küçültme düğmelerinin gösterilip gösterilmeyeceğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

Genişlet/küçült düğmelerinin gösterilip gösterilmeyeceğini alır ve ayarlar.

```csharp
public bool ShowDrill { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDrillDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle ve örnek veri ile doldur
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Pivot";
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B4"].Value = 150;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Drilldown'ı etkinleştir ve drill göstergelerini göster
            pivotTable.EnableDrilldown = true;
            pivotTable.ShowDrill = true;
            
            // Verileri yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableShowDrillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


