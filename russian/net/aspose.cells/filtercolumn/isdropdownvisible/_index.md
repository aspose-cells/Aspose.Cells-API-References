---
title: "FilterColumn.IsDropdownVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Указывает, видна ли кнопка AutoFilter для этого столбца"
type: docs
url: /ru/net/aspose.cells/filtercolumn/isdropdownvisible/
---
## FilterColumn.IsDropdownVisible property

Указывает, видна ли кнопка AutoFilter для этого столбца.

```csharp
public bool IsDropdownVisible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyIsDropdownVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["A4"].PutValue("Fruit");

            // Применить AutoFilter
            sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string

            // Получите столбец фильтра
            FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

            // Показать выпадающий список изначально
            filterColumn.IsDropdownVisible = true;
            Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");

            // Скрыть выпадающий список
            filterColumn.IsDropdownVisible = false;
            Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");

            // Сохраните книгу
            workbook.Save("FilterColumnDropdownDemo.xlsx");
        }
    }
}
```

### См. также

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


