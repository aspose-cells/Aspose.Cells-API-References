---
title: "AutoFilter.ShowFilterButton"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter özelliği. Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/autofilter/showfilterbutton/
---
## AutoFilter.ShowFilterButton property

Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir.

```csharp
public bool ShowFilterButton { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyShowFilterButtonDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Bir liste nesnesi/tablo oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];

            // Otomatik filtreyi etkinleştir ve filtre düğmelerini göster
            table.AutoFilter.ShowFilterButton = true;

            // Çalışma kitabını kaydedin
            workbook.Save("output_with_filter_buttons.xlsx");

            // Filtre düğmelerini gizle
            table.AutoFilter.ShowFilterButton = false;
            workbook.Save("output_without_filter_buttons.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


