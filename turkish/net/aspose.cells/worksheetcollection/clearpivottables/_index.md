---
title: "WorksheetCollection.ClearPivottables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Elektronik tablodan pivot tabloları temizler"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/clearpivottables/
---
## WorksheetCollection.ClearPivottables method

Pivot tablolarını elektronik tablodan temizler.

```csharp
public void ClearPivottables()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodClearPivottablesDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Bir pivot tablo ekle
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            Console.WriteLine("Pivot tables count before clearing: " + worksheet.PivotTables.Count);

            // Tüm çalışma sayfalarındaki tüm pivot tabloları temizle
            workbook.Worksheets.ClearPivottables();

            Console.WriteLine("Pivot tables count after clearing: " + worksheet.PivotTables.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


