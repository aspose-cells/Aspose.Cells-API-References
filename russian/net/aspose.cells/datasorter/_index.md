---
title: "Класс DataSorter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DataSorter. Краткое описание для DataSorter"
type: docs
url: /ru/net/aspose.cells/datasorter/
---
## DataSorter class

Краткое описание для DataSorter.

```csharp
public class DataSorter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | Получает и задает, учитывается ли регистр при сравнении строк. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | Представляет, имеет ли диапазон заголовки. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | Представляет индекс первого отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | Представляет индекс второго отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | Представляет индекс третьего отсортированного столбца (абсолютная позиция, столбец A — 0, B — 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | Получает список ключей сортировщика данных. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | Представляет порядок сортировки первого ключа. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | Представляет порядок сортировки второго ключа. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | Представляет порядок сортировки третьего ключа. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | Указывает, сортировать ли всё, что выглядит как число. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | True означает, что ориентация сортировки слева направо. False означает, что ориентация сортировки сверху вниз. Значение по умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | Добавляет ключ сортировки по цвету. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | Добавляет индекс отсортированного столбца и порядок сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | Добавляет индекс отсортированного столбца и порядок сортировки с пользовательским списком сортировки. |
| [Clear](../../aspose.cells/datasorter/clear/)() | Очистить все настройки. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | Отсортировать данные в диапазоне. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | Отсортировать данные области. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | Сортирует данные области. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterDemo
    {
        public static void DataSorterExample()
        {
            // Создать новый объект Workbook
            Workbook workbook = new Workbook("DataSorter_original.xlsx");

            // Получить объект DataSorter рабочей книги
            DataSorter sorter = workbook.DataSorter;

            // Установить первый порядок для объекта DataSorter
            sorter.Order1 = SortOrder.Descending;
            // Определить первый ключ
            sorter.Key1 = 0;

            // Установить второй порядок для объекта DataSorter
            sorter.Order2 = SortOrder.Ascending;
            // Определить второй ключ
            sorter.Key2 = 1;

            // Создать область ячеек (диапазон)
            CellArea ca = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 13,
                EndColumn = 1
            };

            // Отсортировать данные в указанном диапазоне (A1:B14)
            sorter.Sort(workbook.Worksheets[0].Cells, ca);

            // Сохранить файл Excel
            workbook.Save("DataSorterExample.xlsx");
            workbook.Save("DataSorterExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


