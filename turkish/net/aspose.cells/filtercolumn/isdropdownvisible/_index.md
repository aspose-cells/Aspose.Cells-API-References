---
title: "FilterColumn.IsDropdownVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FilterColumn özelliği. Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/filtercolumn/isdropdownvisible/
---
## FilterColumn.IsDropdownVisible property

Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir.

```csharp
public bool IsDropdownVisible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyIsDropdownVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["A4"].PutValue("Fruit");

            // AutoFilter'ı uygula
            sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string

            // Filtre sütununu alın
            FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

            // Açılır menüyü başlangıçta göster
            filterColumn.IsDropdownVisible = true;
            Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");

            // Açılır menüyü gizle
            filterColumn.IsDropdownVisible = false;
            Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");

            // Çalışma kitabını kaydedin
            workbook.Save("FilterColumnDropdownDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


