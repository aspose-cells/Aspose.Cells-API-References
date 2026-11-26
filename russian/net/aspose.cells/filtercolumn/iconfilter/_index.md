---
title: "FilterColumn.IconFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Возвращает IconFilter для фильтрации данных по значку"
type: docs
url: /ru/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

Возвращает `IconFilter` для фильтрации данных по значку.

```csharp
public IconFilter IconFilter { get; }
```

### Примечания

Перед использованием этого свойства, пожалуйста, убедитесь, что [`FilterType`](../filtertype/) установлен в IconFilter, иначе будет возвращено null.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте образцовые данные с условным форматированием, использующим значки
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // Применить автофильтр к диапазону
                worksheet.AutoFilter.Range = "A1:A5";

                // Получите столбец фильтра
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Получите доступ к свойству IconFilter (только для чтения)
                IconFilter iconFilter = filterColumn.IconFilter;

                // Отобразить свойства IconFilter, если они существуют
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // Сохраните книгу
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
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

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


