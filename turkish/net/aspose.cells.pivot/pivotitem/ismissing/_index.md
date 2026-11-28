---
title: "PivotItem.IsMissing"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotItem özelliği. Öğenin veri kaynağından kaldırılıp kaldırılmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.pivot/pivotitem/ismissing/
---
## PivotItem.IsMissing property

Öğenin veri kaynağından kaldırılıp kaldırılmadığını gösterir.

```csharp
public bool IsMissing { get; }
```

### Açıklamalar

True, bu değerin veri kaynağından kaldırıldığını gösterir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsMissingDemo
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
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Özet tablo verilerini yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // İlk satır alanındaki ilk pivot öğesini al
            PivotField rowField = pivotTable.RowFields[0];
            PivotItem pivotItem = rowField.PivotItems[0];

            // IsMissing özelliği değerini göster
            Console.WriteLine("IsMissing value for '{0}': {1}", pivotItem.Name, pivotItem.IsMissing);

            // Bir öğenin eksik olabileceği bir senaryo oluştur
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B5"].PutValue(4000);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Orijinal pivot öğesinin artık eksik olup olmadığını kontrol et
            Console.WriteLine("After data change - IsMissing value for '{0}': {1}", 
                pivotItem.Name, pivotItem.IsMissing);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotItemIsMissingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


