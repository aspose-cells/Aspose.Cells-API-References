---
title: "PivotField.RegionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Bu alanın görüntülendiği pivot tablo bölgesini belirtir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/regiontype/
---
## PivotField.RegionType property

Bu alanın görüntülendiği pivot tablo bölgesini belirtir.

```csharp
public PivotFieldType RegionType { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyRegionTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Bir pivot tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Özet tablo verilerini yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // İlk pivot alanını al
            PivotField pivotField = pivotTable.RowFields[0];

            // Mevcut RegionType değerini göster
            Console.WriteLine("Current RegionType value: " + pivotField.RegionType);

            // RegionType özelliğinin nasıl kullanılacağını göster
            if (pivotField.RegionType == PivotFieldType.Row)
            {
                Console.WriteLine("This pivot field is in the row area");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldRegionTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


