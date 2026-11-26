---
title: "FilterColumn.ColorFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Получает ColorFilter для фильтрации данных по цвету"
type: docs
url: /ru/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

Получает [`ColorFilter`](../../colorfilter/) для фильтрации данных по цвету.

```csharp
public ColorFilter ColorFilter { get; }
```

### Примечания

Устанавливает [`FilterType`](../filtertype/) как ColorFilter первым, иначе будет возвращён Null.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавить примерные данные с цветами
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // Применить автофильтр
                worksheet.AutoFilter.Range = "A1:A4";

                // Получите столбец фильтра
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Получить доступ к свойству ColorFilter (только для чтения)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // Отобразить свойства ColorFilter
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // Сохраните книгу
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
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

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


