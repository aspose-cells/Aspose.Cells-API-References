---
title: "Перечисление SortOnType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.SortOnType. Тип сортируемого значения"
type: docs
url: /ru/net/aspose.cells/sortontype/
---
## SortOnType enumeration

Тип отсортированного значения.

```csharp
public enum SortOnType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Value | `0` | Сортирует по значению ячеек. |
| CellColor | `1` | Сортирует по цвету ячеек. |
| FontColor | `2` | Сортирует по цвету шрифта ячеек. |
| Icon | `3` | Сортирует по условному значку. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SortOnTypeDemo
    {
        public static void SortOnTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(95);
            worksheet.Cells["B4"].PutValue(75);

            // Применить автофильтр к диапазону
            worksheet.AutoFilter.Range = "A1:B4";

            // Получить автофильтр
            AutoFilter autoFilter = worksheet.AutoFilter;

            // Получить сортировщик данных
            DataSorter sorter = autoFilter.Sorter;

            // Установить первый ключ сортировки по значениям во второй колонке (Score)
            sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);

            // Отсортировать данные в диапазоне
            sorter.Sort(worksheet.Cells, 1, 0, 3, 1);

            // Сохраните книгу
            workbook.Save("SortOnTypeExample.xlsx");

            // Выведите результаты
            Console.WriteLine("Data sorted by Score in descending order.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


