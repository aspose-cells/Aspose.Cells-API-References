---
title: "PivotField.DisplayName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Pivot tablo görünümünde pivot alanının görüntüleme adını temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Pivot tablo görünümünde pivot alanının görüntülenen adını temsil eder.

```csharp
public string DisplayName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Veri alanı için özel görüntüleme adı ayarla
            pivotTable.DataFields[0].DisplayName = "Total Sales";
            
            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Görüntüleme adı kullanarak hücreye eriş
            Cell cell = pivotTable.GetCellByDisplayName("Total Sales");
            Console.WriteLine("Cell found at row: {0}, column: {1}", cell.Row, cell.Column);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotFieldDisplayNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


