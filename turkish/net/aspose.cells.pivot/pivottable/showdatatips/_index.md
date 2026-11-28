---
title: "PivotTable.ShowDataTips"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Araç ipuçlarının PivotTable veri hücrelerinde gösterilip gösterilmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/showdatatips/
---
## PivotTable.ShowDataTips property

PivotTable veri hücreleri için araç ipuçlarının gösterilip gösterilmeyeceğini gösterir.

```csharp
public bool ShowDataTips { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDataTipsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ve bazı örnek veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 20;

            // Bir pivot tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Veri ipuçlarını etkinleştir
            pivotTable.ShowDataTips = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableWithDataTips.xlsx");
            
            Console.WriteLine("Pivot table with ShowDataTips enabled created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


