---
title: "Класс IconFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.IconFilter. Представляет фильтр значков"
type: docs
url: /ru/net/aspose.cells/iconfilter/
---
## IconFilter class

Представляет фильтр значков.

```csharp
public class IconFilter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | Получает и задает нулевой индекс значка в наборе значков. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Получает и задает набор значков, используемый для этого критерия фильтра. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Заполнить примерными данными
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // Создать автофильтр
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // Получить фильтр значков
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // Установить свойства фильтра значков
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // Сохраните книгу
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon filter applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with IconFilter: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


