---
title: "PivotTable.MergeLabels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Birden fazla hücreyi kapsayan satır/sütun alan etiketlerini birleştirip birleştirilmeyeceğini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/mergelabels/
---
## PivotTable.MergeLabels property

Birden çok hücreye yayılan satır/sütun alan etiketlerinin birleştirilip birleştirilmeyeceğini alır veya ayarlar.

```csharp
public bool MergeLabels { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMergeLabelsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Apple";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Orange";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Etiket birleştirmeyi etkinleştir
            pivotTable.MergeLabels = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableMergeLabelsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


