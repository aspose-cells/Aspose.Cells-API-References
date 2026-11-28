---
title: "Worksheet.Slicers"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasındaki Slicer koleksiyonunu al"
type: docs
url: /tr/net/aspose.cells/worksheet/slicers/
---
## Worksheet.Slicers property

Çalışma sayfasındaki Slicer koleksiyonunu al.

```csharp
public SlicerCollection Slicers { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySlicersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tablo için örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Bir tablo ekle
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Çalışma sayfasına dilimleyiciler ekle
            worksheet.Slicers.Add(table, table.ListColumns[0], 1, 3);
            worksheet.Slicers.Add(table, 1, "D1");
            worksheet.Slicers.Add(table, table.ListColumns[0], "G1");

            // Çalışma kitabını kaydedin
            workbook.Save("SlicersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


