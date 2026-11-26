---
title: "FilterColumn.FieldIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Получает и задает смещение столбца в диапазоне"
type: docs
url: /ru/net/aspose.cells/filtercolumn/fieldindex/
---
## FilterColumn.FieldIndex property

Получает и задает смещение столбца в диапазоне.

```csharp
public int FieldIndex { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Employees");
            worksheet.Cells["A2"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["A3"].PutValue("Marketing");
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["A4"].PutValue("IT");
            worksheet.Cells["B4"].PutValue(12);

            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:B4";
            
            // Добавить фильтр в первый столбец (Department)
            worksheet.AutoFilter.AddFilter(0, "Sales");

            // Получите столбец фильтра
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            
            // Продемонстрировать свойство FieldIndex
            Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
            
            // Обновить и сохранить
            worksheet.AutoFilter.Refresh();
            workbook.Save("FilterColumnFieldIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


