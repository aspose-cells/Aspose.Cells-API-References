---
title: "PivotField.ShowAllItems"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Özet veri içermeseler bile PivotTable görünümünde tüm öğelerin gösterilip gösterilmeyeceğini belirler. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Özet veri içermeseler bile PivotTable görünümünde tüm öğelerin gösterilip gösterilmeyeceğini belirtir. Varsayılan değer false'tur.

```csharp
public bool ShowAllItems { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowAllItemsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Product");
            sheet.Cells["C1"].PutValue("Sales");
            
            sheet.Cells["A2"].PutValue("Electronics");
            sheet.Cells["B2"].PutValue("Laptop");
            sheet.Cells["C2"].PutValue(1200);
            
            sheet.Cells["A3"].PutValue("Electronics");
            sheet.Cells["B3"].PutValue("Phone");
            sheet.Cells["C3"].PutValue(800);
            
            sheet.Cells["A4"].PutValue("Furniture");
            sheet.Cells["B4"].PutValue("Chair");
            sheet.Cells["C4"].PutValue(150);

            // Pivot tablo ekle
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Satır alanı için ShowAllItems özelliğini ayarla
            PivotField rowField = pivotTable.RowFields[0];
            rowField.ShowAllItems = true;

            // Verileri hesaplayın ve kaydedin
            pivotTable.CalculateData();
            workbook.Save("PivotFieldShowAllItemsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


