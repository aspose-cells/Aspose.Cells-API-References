---
title: "FilterColumn.FieldIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Aralıktaki sütun ofsetini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/filtercolumn/fieldindex/
---
## FilterColumn.FieldIndex property

Aralıktaki sütun kaydırmasını alır ve ayarlar.

```csharp
public int FieldIndex { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Employees");
            worksheet.Cells["A2"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["A3"].PutValue("Marketing");
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["A4"].PutValue("IT");
            worksheet.Cells["B4"].PutValue(12);

            // Otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:B4";
            
            // İlk sütuna (Departman) filtre ekle
            worksheet.AutoFilter.AddFilter(0, "Sales");

            // Filtre sütununu alın
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            
            // FieldIndex özelliğini göster
            Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
            
            // Yenile ve kaydet
            worksheet.AutoFilter.Refresh();
            workbook.Save("FilterColumnFieldIndexDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


