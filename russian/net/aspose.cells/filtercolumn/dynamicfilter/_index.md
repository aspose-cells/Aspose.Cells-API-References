---
title: "FilterColumn.DynamicFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Получает DynamicFilter для фильтрации с динамическими критериями"
type: docs
url: /ru/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

Получает `DynamicFilter` для фильтрации с динамическими критериями.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### Примечания

Перед использованием этого свойства убедитесь, что [`FilterType`](../filtertype/) установлен в DynamicFilter, иначе будет возвращено null.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте примерные данные
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // Применить автофильтр
                worksheet.AutoFilter.Range = "A1:A4";

                // Получите столбец фильтра
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Доступ к свойству DynamicFilter (только для чтения)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // Отобразить свойства DynamicFilter
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // Сохраните книгу
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


