---
title: "PivotTable.RowGrand"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Bu pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/rowgrand/
---
## PivotTable.RowGrand property

Bu pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini belirtir.

```csharp
[Obsolete("Use PivotTable.ShowRowGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool RowGrand { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.ShowRowGrandTotals yöntemini kullanın. Bu yöntem, Aralık 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRowGrandDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            
            worksheet.Cells["A5"].PutValue("Product A");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(1500);
            
            worksheet.Cells["A6"].PutValue("Product B");
            worksheet.Cells["B6"].PutValue("North");
            worksheet.Cells["C6"].PutValue(2500);

            // Bir pivot tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C6", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // RowGrand'ın mevcut değerini göster
            Console.WriteLine("Current RowGrand value: " + pivotTable.RowGrand);

            // RowGrand özelliğini değiştir
            pivotTable.RowGrand = false;

            // Pivot tablo verilerini hesapla
            pivotTable.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTablePropertyRowGrandDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


