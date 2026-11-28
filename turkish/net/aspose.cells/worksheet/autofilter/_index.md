---
title: "Worksheet.AutoFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Belirtilen çalışma sayfası için otomatik filtreyi temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Belirtilen çalışma sayfası için otomatik filtreyi temsil eder.

```csharp
public AutoFilter AutoFilter { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Shirt");
            worksheet.Cells["B3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Phone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["A5"].PutValue("Pants");
            worksheet.Cells["B5"].PutValue("Clothing");

            // Otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.Filter(1, "Electronics");

            // Filtreyi yenile
            worksheet.AutoFilter.Refresh();

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


