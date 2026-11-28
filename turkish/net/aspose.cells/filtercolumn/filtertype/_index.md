---
title: "FilterColumn.FilterType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Filtreleme verisinin türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

Veri filtreleme türünü alır ve ayarlar.

```csharp
public FilterType FilterType { get; set; }
```

### Açıklamalar

Bu özellik ayarlandığında ilgili filtre nesnesi oluşturulacak ve ilgili özellik, filtre nesnesini buna göre almak için kullanılmalıdır:

| **FilterType** | **Property** |
| --- | --- |
| MultipleFilters | [`FilterValues`](../filtervalues/) |
| CustomFilters | [`CustomFilters`](../customfilters/) |
| ColorFilter | [`ColorFilter`](../colorfilter/) |
| DynamicFilter | [`DynamicFilter`](../dynamicfilter/) |
| IconFilter | [`IconFilter`](../iconfilter/) |
| Top10 | [`Top10Filter`](../top10filter/) |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("HR");
            sheet.Cells["A3"].PutValue("IT");
            sheet.Cells["A4"].PutValue("Finance");

            sheet.Cells["B1"].PutValue("Employees");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(15);
            sheet.Cells["B4"].PutValue(8);

            // Dize aralığı kullanarak otomatik filtre uygula
            sheet.AutoFilter.Range = "A1:B4";

            // Farklı filtre türleri ekleyerek FilterType özelliğini göster
            sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
            sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter

            // Filtre sütunlarını al
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Her sütun için FilterType'ı göster
            for (int i = 0; i < filterColumns.Count; i++)
            {
                FilterColumn filterColumn = filterColumns[i];
                Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("FilterTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


