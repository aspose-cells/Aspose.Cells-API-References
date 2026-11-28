---
title: "PivotTable.ManualUpdate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. PivotTable raporunun yalnızca kullanıcının isteği üzerine yeniden hesaplanıp hesaplanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/manualupdate/
---
## PivotTable.ManualUpdate property

**PivotTable** raporunun yalnızca kullanıcının talebi üzerine yeniden hesaplanıp hesaplanmayacağını gösterir.

```csharp
public bool ManualUpdate { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyManualUpdateDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle ve örnek veri ile doldur
            Worksheet dataSheet = workbook.Worksheets["Sheet1"];
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["A4"].PutValue("A");
            dataSheet.Cells["B4"].PutValue(30);

            // Bir pivot tablo ekle
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int index = pivotSheet.PivotTables.Add("Sheet1!A1:B4", "A3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];

            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Manuel güncellemeyi etkinleştir
            pivotTable.ManualUpdate = true;
            
            // Bu noktada, pivot tablo otomatik olarak yenilenmeyecek
            Console.WriteLine("Pivot table before refresh (ManualUpdate=true):");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will be empty
            
            // Pivot tabloyu manuel olarak yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            Console.WriteLine("Pivot table after manual refresh:");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will show "40" (sum of category A)
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableManualUpdateDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


