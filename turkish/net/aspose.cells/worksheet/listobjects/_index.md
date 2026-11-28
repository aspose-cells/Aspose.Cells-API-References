---
title: "Worksheet.ListObjects"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bu çalışma sayfasındaki tüm ListObject'leri alır"
type: docs
url: /tr/net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Bu çalışma sayfasındaki tüm ListObject'leri alır.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyListObjectsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Bir ListObject (tablo) oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.DisplayName = "ProductTable";
            table.ShowTotals = true;
            
            // Tablonun daha fazla satır içerecek şekilde boyutunu değiştir
            table.Resize(table.StartRow, table.StartColumn, 5, table.EndColumn, true);
            
            // Genişletilmiş tabloya daha fazla veri ekleyin
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["A5"].PutValue("Item4");
            worksheet.Cells["B5"].PutValue(400);
            
            // Tabloya ListObjects özelliği aracılığıyla erişin
            ListObject retrievedTable = worksheet.ListObjects["ProductTable"];
            retrievedTable.ShowHeaderRow = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ListObjectsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


