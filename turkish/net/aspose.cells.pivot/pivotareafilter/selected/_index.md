---
title: "PivotAreaFilter.Selected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotAreaFilter özelliği. Bu alanın seçili olup olmadığını gösterir. Yalnızca PivotTable Taslak görünümünde çalışır."
type: docs
url: /tr/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

Bu alanın seçimi olup olmadığını gösterir. Yalnızca PivotTable Taslak görünümünde çalışır.

```csharp
public bool Selected { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Bir pivot tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Pivot alan filtresini al.
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // Mevcut Selected değerini göster.
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // Selected değerini değiştir (yalnızca Taslak görünümü etkiler).
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


